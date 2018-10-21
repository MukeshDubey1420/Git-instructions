In the programming world, it is necessary to understand and manage the versions of your code and projects that you create working hard day and night. In This Documentation  I will introduce you to **Git and GitHub**, one of the prominent and famous version control system used by most of the developers across the globe, some basic Git commands, and how to set up your local and remote repository on GitHub using the terminal of mac computer.

## What is Git and GitHub?
When it comes to Git and Github, most people get confused and think that both are more or less the same thing but, Git is a free and open source distributed version control system whereas GitHub is an online hosted platform for various services.

![Git](Screenshots/gitgithub.png)

Suppose, initially, you created a file say ABC.txt within a folder on your system. Using the concepts of version control, you can manage, track, commit changes, roll back to a previous safe state and much more easily. In the above diagram, the local file can be converted to trackable files i.e a version control system using Git commands. Why is version control Important?

While programming and as a human, it is our tendency to make mistakes and then land up ourselves in a  position from where coming back to original state is not possible and we are lost. Using version control, we can track and control our huge files full of codes very easily and quickly

# **What is Git ??**
#### Git is Created by **_Linus Trovaldus_**.(responsible for the linux kernel.)
##### Git is a version control system (VCS). Git is a tool/software like your IDE or VLC player. It is not a programming language.It is a general tool.Chances For Hiring In a Company will be increased When u Mentioned Git ON ur Resumes.
* Image of the **_Linus Trovaldus_** Is Shown Below.

 * ( He is the Creator, and for a long time, principal developer of the Linux kernel, which became the kernel for operating systems such as the Linux operating system, Android, and Chrome OS. **He also created the distributed revision control system Git**)

![LinusTrovaldus](Screenshots/Linustrovalds.jpg)

# What Git Does ??
There are two main Reasons to Learn GIT.
1. Track changes to your code .
2. Save your code to the cloud .

# What is GitHub ??
The Term Git & Github are not same. Github is a website/platform while git is a tool/Software.
For Ex:- *Git or Camera is just the tool, But Instagram or GitHub is the website.*
**Github allows you to safely store your code in the cloud. And Also U can Share Your Code With Others.**

There Are also Other websites such as gitlab, bitbucket which are similar to Github also exists . **Companies love it when you have a github profile and they can see your work before even calling you for an interview.**
* Now the Question Arises We Can do the same from Google Drive or DropBox, But the Solution is It Is Designed for special purpose(It even Track the record of code that u wrote 5 years ago. And what is it.)

### **Installation Steps For Git and GitHub , How to Create Repository, Add And Commit Your Code And How Push It On GitHub Using Git.**

## Pre-requisites (Basic Requirements.)
##### 1. **Git Installed In your System**. To Install Git [Click here.](https://git-scm.com/) U Will See below, what appears Next and what we Have to Do Next.

![git download](Screenshots/git.PNG)
* After Downloading Simply Run the setup file, And click **Next**

![git file](Screenshots/1st.PNG)

* Check 2nd checkbox as shown and click **Next**

![checkbox](Screenshots/2nd.PNG)

* Check with **_use the native window secure channel library_** and click **Next**

![windowcheckbox](Screenshots/3rd.PNG)

* Check with **_use MinTTY_** and click **Next**

![checkboxlast](Screenshots/4th.PNG)

* Check first two checkbox and click **Next**

![checkboxx](Screenshots/5th.PNG)

* After That Installation process Start, Wait for Complete setup To Finish.

![Installation](Screenshots/6th.PNG)

* **Now Ur Git has Installed SuccessFully.**

##### 2. **A GitHub Account** . If you don't have Account on GitHub,Create it By [Clicking here.](https://github.com/join) Make sure your username is professional (Just similar like creating an account on instagram or on facebook,also verify your email and mobile no.)  Note:- *coolsmartboy1994 or dhinchakpooja does not work.*


#### After Creating Account and Signing In, U Just have to **Create New Repository on Github**.

1. Open your Github account . You will see a page somewhat like this .

![new repository](Screenshots/newrepo.PNG)
2. Click on **Start Project** Button to create a new project repository.Or you can also click on the **new repository** as shown in the bottom corner of the image to Create a Repo.

3. Once you have clicked you'll be directed to this page.

![new repo1](Screenshots/newrepo1.PNG)

4. Enter the repository name you want to set. **Remember, There are some conventions to naming the repositories** . When you enter the name wait for a while until the green tick comes as shown in the image, Description field is optional.

5. Then you can Click on the green **create Repository** button. (As shown Below)

6. Then you will be Redirected to the Next Page.

![newrepo3](Screenshots/newrepo3.PNG)

7. Now You **Succesfully** created a New Repository on GitHub .**This Github Repo is often referred to as Remote repo**. It Is Called So Because it is not close to you, it is remote, it is on the cloud.Every project needs one remote repository for itself.

8. Now we will see how we can **_push_** our data from Local Repository(The one which contains your project file into the system) into the Remote Repository (The one which you created online on GitHub).

## It Can Be Done by Using Basic Git Commands.

1. Once you have installed Git on your system we can push our projects through it.

2. Open Git Bash and The Window Will Appears Something like this.
 ![git bash](Screenshots/git1.PNG)
3. The First two commands you need to run are just to get youself registered on Git.
```   
 git config --global user.name "Your GitHub UserName"

 git config --global user.email "Your Valid Email-Id"
```
![git2](Screenshots/git2.PNG)    
Note:-  **Make sure the username and email you entered are  Github registered** (_not necessary but makes work easy_)

4. Now you need to direct your Git Bash to **The designated folder(Local Repository) In Which Project Related Files or your Assignments Are Present Which u want to Push On Github Remote Repository .**  For that we use the ```cd "path"```  command (Change Directory).
   In the double quotes you need to enter the full path of your Local Repository.

   ![git path](Screenshots/git3.PNG)

5.  Now we have reached at our project folder(Local Repository) the first thing  we need to do is  initialise An Empty Repository (as .git) in the Local Repository (Project Folder) .`git init` just like git k folder mein greh pravesh krna.

                or

This command is used to create a git local repository of your file and then you can start tracking the changes you make in the future. This command initializes an empty git repository inside the same directory that you are currently in with .git extension eg. of code on the terminal
```
git init
```   
![gitinit](Screenshots/git4.PNG)

By Using this `git init` command, It will make a .git folder in your Local Repository.(Git creates a hidden folder called .git inside a folder that you want to track. Just this much makes a folder into a git repository.) and creates a Master Branch for Git To track the Files. As u can See Below.

![gitnew](Screenshots/git5.PNG)

6 . Till Now we have created the .git folder . Now We have to add the files , It can be done in two ways:
* Using Selectively Approach.(In case u Wanna to Add Only a Specific Files out of bunch of many Files Present in ur local repository.)
```python
git add filename
```
* By Addding All Files.(In case u wanna to Add all the files and Folders which are present in your local repository)
```python
git add .
```
7 . Here We will use the `git add .`command, But u can also try Selective approach too.

![git add . ](Screenshots/git6.PNG)

8 . Once we have added the files in repo, the next thing we need to do is commit these changes By using `git commit` command and provide a message with commit .Commits are like check points or versions of your software.Even a new single line added to your code can count as a new version.So after you add the file you need to do a commit to make a version out of it.	Commit changes to head (but not yet to the remote repository):
Let's create the first commit or first version of our project:
```python

git commit -m "your commit message"

```
**Remember:** _The commit message should be a meaningful one ._  Like:-
1. The Bug is resolved.
2. Code has been Improved.
3. Additional Features are added (Mention it).
4. Files Are added via Upload.

![git commit](Screenshots/git7.PNG)

*9*.  Next we will connect our GitHub Remote Repo with Local Repository using the link given to us on the github page. (Just Like providing the path where this data is to be stored or Simply Mapping It.)

 ![github link](Screenshots/git8.PNG)
 **Copy the blue highlighted part**

10 .If you haven't connected your local repository to a remote server, add the server to be able to push to it: For this we will use the HTTPS Url Link to Map or to Link our Local Repository to Remote Repository.

*11*. For that we will use `git remote add origin 'paste your copied URI Link here'` command.
```python
git remote add origin 'paste that Copied Link here'

```

![git remote add](Screenshots/git9.PNG)

12 . The last step is to **_push_** the Project Files to the Remote repository.And For that We will use `git push origin master` command. It Sends changes to the master branch of your remote repository:

**Note :- At this Stage you must have internet connection connected with your system otherwise it will throw an error _host could not resolved_ so make sure net has connected.**
  ```python

git push origin master

```
![git ](Screenshots/git10.PNG)


13 . If everything you have done is correct and followed the Steps correctly your github repository should have been updated.(Sometimes it would accept username and password then simply after providing username nd password files are uploaded),**Now Simply Refresh ur Browser and u will see that the Files are Added to GitHUB Remote repo From Local Repo.**

![gitrepo](Screenshots/git11.PNG)
_It will shows something like this_

*14*.  In some Of the cases when you push the code, you might have to sign up .

 **Remember** : **_when Pushing your code to Github, Ur system is connected to Internet and the network should be working_**, Otherwise u have to face internet connection Error.

 Note:- Only Push command Requires Internet connection.

*15*. For the next times you just need to remember these commands _in this order_
 ```python
git add .
git commit -m "your message"
git push origin master

```

*16*. Some other useful commands are :

1.`git log` tells the no. of commits,commit history,gives commit id(**A commit id. Think of this as a unique version id which uniquely identifies that version of the commit. This is an alpha-numeric string. Ex: ca82a6dff817ec66f44342007202690a93763949**), and also shows the provided message along with that date and time on which commit has been done.
 ```python
git log #tells the log of your commits
```
![gitlog](Screenshots/gitlog.PNG)

*2*.`git status` it Lists the files you've changed and those you still need to add or commit:
it is a very useful command which tells us the status of the file which is being tracked(added)or not.The command tells you the current state of your project. It is like a report card of your project.
You will discover more about it as you start using git more and more.
```python

git status # used to know the status of the files being tracked or not

```
![git status](Screenshots/gitstatus.PNG)
* now add more files to our project like: new.txt, main.txt(`git add new.txt`,`git add main.txt`)
* Also add some content in ur previous project files and the newly added files main.txt and new.txt*
* Now run the git status command,git will track the modified files too . now u have to again commit it via providing meaning message that file is modified .

**Please note that you have to add both new and modified files before you can make a new commit or version. That is you will need to tell git what all files are a part of the commit/version everytime. This is super important!!**

* Now push ur code to Github again.

17 . I hope all these Things are cleared to u ,,`Thank you .`

# A quick Revision of the used commands.
* `git init` - Create an empty git repository
* `git add .` - Add all files to the next commit/version
* `git status` - Gives the status for thr files which are tracked,untracked and modified.
* `git commit -m "Your meaningful message here"` - Create a commit/version of the proejct
* `git log` - See commit/version history of the project
* `git remote add origin 'Paste your link for remote repo here'` to add the link btw remote repo and local repo.
* `git push origin master` - To push your code ,your project project file to Remote repo from local repo.

## Additional Commands (Branching , Cloning , Merging Pull Requests)..

* `git clone /path/to/repository`  - **Check out a repository** --- It Creates a working copy of a local repository.

* `git remote -v` - It Displays the List all currently configured remote repositories.

* `git checkout -b <branchname>` **Branches** -- It Creates a new branch and switch to it.

* `git branch` It Lists all the branches in your repo, and also tell you what branch you're currently in.

* `git checkout <branchname>`  it Switches from one branch to another.

* `git branch -d <branchname>` it Deletes the feature branch:

* `git push origin <branchname>` it Pushes the branch to your remote repository, so others can use it.

* `git push --all origin` it Pushes all branches to your remote repository:

* `git pull origin master` it will pull changes from the origin remote, master branch and merge them to the local checked-out branch.

Note :- By doing so Sometimes Vim editor opens , Command is `:wq` ":" enter ,"w" write , "q" save and quit.

* `git merge <branchname>` it is used to To merge a different branch into your active branch:
 
* `git stash` it is used to stash or store the entire work on a stack and working directory will be clean.

* `git stash pop` it is used to un-apply the stashed items from git and everything will be back.
