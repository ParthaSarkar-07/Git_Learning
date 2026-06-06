# Git_Learning
I just have learned about the git na fthe github. How to use thw git in the real world projects and keep track of them and puah the code to the github.



# **INTODUCTION**:

>  **Git** is ==a distributed version control system that tracks changes in computer files and coordinates work among multiple developers==. It functions like a "checkpoint" or snapshot system, allowing you to save different versions of your project, collaborate without overriding others' work, and easily revert to previous states if mistakes occur.

>  ==**Linus Torvalds**==, the creator of the Linux operating system, created Git in **April 2005**.

>  The Linux kernel development team had been using a proprietary source control tool called ==**BitKeeper**==. When a licensing dispute occurred and the tool's free-of-charge status was revoked, Torvalds needed a new tool immediately.
  
<img width="347" height="145" alt="Git" src="https://github.com/user-attachments/assets/7595cd86-71ef-4f0c-bc11-4a9d8098fde2" />

## **Git Init:**  
   
  >The `git init` command is used to initialize a new repository. The instructor emphasizes that this should only be run **once per project** to create the necessary hidden `.git` directory, which houses the repository's internal tracking mechanisms. 

## **Tracking Status:** 

  >By using `git status`, you can verify whether a folder is being tracked by Git. After initialization, the output changes from an error message to a confirmation that the directory is now under Git's management .

## **Workflow Philosophy:**
   
  >The core takeaway is that Git is a powerful tool for managing version history, and understanding these foundational commands allows developers to maintain clean and reliable project workflows without needing to rely on trial-and-error. 
# **Git Commit and Log:**


<img width="585" height="434" alt="git intro" src="https://github.com/user-attachments/assets/08a5018e-73f6-4d49-b5be-0a1e0e35c5f3" />

<img width="586" height="438" alt="git initialise preccess" src="https://github.com/user-attachments/assets/85f310c8-84d3-446c-9436-f0b332eb66a6" />

<img width="379" height="424" alt="version_control_flowchart" src="https://github.com/user-attachments/assets/37be2412-7da1-4de0-ad43-5b5b6e42954e" />


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
<img width="755" height="447" alt="gitlog" src="https://github.com/user-attachments/assets/e95004d7-daf8-4554-95c1-923326aa84e7" />



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


<img width="805" height="559" alt="git commit" src="https://github.com/user-attachments/assets/eff61c39-db38-49db-a15c-2f86d4418cf9" />


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

<img width="823" height="561" alt="Brach" src="https://github.com/user-attachments/assets/843dd7cf-a346-4c92-bdc4-8573565b1f78" />




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
  
<img width="822" height="375" alt="git_branch_command" src="https://github.com/user-attachments/assets/59d5d0b0-1cda-43f1-8662-68f1ecd3cbff" />


## **Git Branch Merge:**


<img width="939" height="639" alt="Git_branch_merge_concept" src="https://github.com/user-attachments/assets/decf87d2-ed5d-4dc9-aa0b-af88c6370c22" />


<img width="903" height="608" alt="some_extar_thing" src="https://github.com/user-attachments/assets/4ee8f01f-1f26-4539-9348-db6b29fc8823" />



>if you want to merge two branch you have to go the branch that you want to merge with 

>so to go to the desire branch 
```sh 
git checkout branch_name1 
```
   and then to merge the branch 
```sh   
git merge branch_name2
```


>>**For Example** i have two branches called `master`(default branch ),`nav_bar` and i want to merge the nav_bar with the master branch. For that we need to commit the changes in each branch first and then 
```sh 
git chechout master 
```
   then 
```sh
git merage nav_bar 
```
   it will look like something that if you are using some git_gui app like (gitlens_extention_vscode, gitkraken_softwere)

<img width="505" height="224" alt="git_merge_show" src="https://github.com/user-attachments/assets/19a27862-866a-432c-9108-307e54334b0b" />


an each dot represent a commit which you can view and it also shows the commit name you can give any commit name it's all about you and your team 


## **Merge Conflict:**
>    
>   Sometime if you are working in the same file in the different branch and you edited the same file differently and at last of all you are wanting to merge the branches then the conflict happen and you can't merge without resolve that.

```sh
git merge footer
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.
```
this will be shown in the terminal

>so when the conflict happen go to you code editor and it will show the conflicts like this.

<img width="478" height="438" alt="conflict" src="https://github.com/user-attachments/assets/ecdaecf3-c981-4812-92b6-e2f63b2af981" />


>>>it also give you a button to solve the conflict or you can do that by yourself.

>>>after you manage the conflict then you can commit the changes in the repo.




# **Git Diff and stashing:**

## **Git Diff:**

<img width="873" height="599" alt="git_diff" src="https://github.com/user-attachments/assets/bd4d2986-af9b-42eb-9c3f-6ea9c46f5d23" />



> >**Git Diff** is a command that allows me to check the difference between the same file of different commit position, different log code, branches and many more thing 

> >let's say you just add a file in the staging area and you want to view the changes you have done from the previous then you can use the command 
```sh
git diff --staged
```

<img width="560" height="459" alt="git_diff_showcase" src="https://github.com/user-attachments/assets/d4af9f0d-1907-4529-a9de-5976ff58a08b" />


## **Git Stash:**

> >Sometime it happens that you are working in the branch and you have to move to the other branch and you don't want to commit the branch then because without commit the file you cant change the branch.  
>
> >At that time you can use the `git stash `command it has so many things but the two commands are used very often
> >`git stash` and `git stash pop`
> 
> >let's think the stash is a voult where you can store the files temporarily by `git stash` and then switch the branch and after your job done you can come and take the files from the voult by `git stash pop` and then you can   just do your work.

```sh
git stash
```

```sh 
git stash pop
```


<img width="880" height="450" alt="Git_stash" src="https://github.com/user-attachments/assets/86c6733e-87ca-4cc0-a1ed-e74262ee5108" />



and you can go back to any of your gcommit by 
```sh
git checkout commit_name or commit_id
```

and if you are want to go back to the original place where you are been then 
```sh
git checkout brach_name 
```
or
```sh
git reflog
```

