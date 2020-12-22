# Repository to learn Github

## Part 1 - Starting up:
1. ### Creating your Local Repo: <br>
   _To start your work with Github, you need to have a local repo. <br>
   Let's create it and prepare your first commit:_
   1. Create the local repsitory: <br>``` git init [GiveANameToYourLocalRepo]```
   2. Enter into your local repo's folder: <br> ```cd [YourLocalRepoName]```
   3. Add an Origin: <br> ``` git remote add origin [your repo url] ```
   4. Create some content inside your local repo <br> ```(as your wish)```
   5. Check the status <br> ```git status```
   6. Stage all untracked files and modifications <br> ```git add . (or the name of the file that You wish)``` 
   7. The first commit:<br> ```git commit -m "[Write the masage for your commit.]"```
2. ### Fetching and pulling: <br> 
   _Now, if You're working in a shared project, You need to synchronize your local repo with the origin repo. To do it, use the command ```"fetch"``` and, after, ```"pull```_.
   1.  ```git fecth origin```
   2.  ```git pull origin```
3. ### Pushing: <br>
   _Now You're able to send your 1st commit to the ```"origin"``` (the remote repo)_.
   1.  ```git push origin master ``` _(or the ```BranchName``` that You could be working on)_.
4. ### Creating a branch: <br>
   _The better way to work with the ```"git flow"``` is via **branches**.<br>In other words, each developer engaged in this project should work in "distinguished box" (**branch**, in the Git language).<br>And after finish your respectives code changes, They need to request a ```"merge"``` into the "master box" (**master branch**, in the Git language)_.
   1.  Create a new branch<br>```git branch BranchName ``` _(or the ```BranchName``` that You wish)_.
   2.  Check all the braches<br>_You'll see an asterisk **(*)** at the left side of your current branch_.<br>```git branch```
   3.  Change from your current branch to the new one<br>```git checkout BranchName```
   4.  Push your new branch to the origin<br>```git push origin BranchName```


Great! Now You're able to make all the code changes that you wish.<br>On the next steps You'll learn how to **delete** some **branch** and how to make a _"pull request"_ to **merge** the changes that You could made in your current **banch** into the project's **master branch**.
____
## Part 2 - Removing some Branch:
1. ### Setting up:<br> 
   _Create a **branch** called **"ToBeDeleted"** and push it into your origin_.
   1.  ```git branch ToBeDeleted```
   2.  ```git push origin ToBeDeleted```
2. ### Deleting a local/remote branch:<br>
   _To delete a remote branch, use the **":"** before the branch name.<br> And to remove a local branch use **"-d"** before tha branch name.<br>e.g.:_
   1. ```git push origin :ToBeDeleted```
   2. ```git branch -d ToBeDeleted```
   <br>Obs.: always use **"-d"** instead **"-D"** to avoid an exclusion of an "unstaged" branch.
____
## Part 3 - The _".gitignore"_:
   * _To avoid the streaming of "unnecessary project's files", like some files that are important only for a specific OS or a specific framework, the Git has the **".gitignore"** facility._
  
   * _To active it, just create a file named **".gitignore"** in the project's root folder, and after that, edit the **".gitignore"** with the **"*.extensions"** or **"./folder/."** that won't be streamed._
   * _After all, if You want a lot of ".gitignore" examples, please visit this [GitHub Repository](https://github.com/github/gitignore)._

____
## Part 4 - Reverting changes made:

_You can revert the changes that You could made with 2 ways:_
### Git revert:
1. Using the command ```git revert <commit-ish>```, used to revert the _"actual code state"_ to the _"code state"_ commited in the ```"<commit-ish>"```. Using the ```git revert```, a new commit will be created with a standard message "revert + [ old ```<commit-ish>``` message ]
   1. _To learn more about ```git revert```, use ```git revert --help```_
   2. _Or visit this [YouTube video](https://youtu.be/6FS0I4CUbK4) (in portuguease)._
### Git reset:
2. Using the command ```git reset [<mode>] [<commit>|fileName]```
   <br>The main modes to ```git reset``` are ```--soft --mixed``` and ```--hard```.
   1. ```--soft``` is used when You just want to exclude the referred commit and it staged files;
   2. ```--mixed``` is the default mode, used when ou wnat to exclude the referred commit <u>**but**</u> don't want to touch on it stage files; and
   3. ```--hard``` is used when You want to remove "everything". Since the commit until all the modification that You cloud mande on each file after the reffered commit.<br>Then, <u>**be careful**</u> when You use it.
### Advice:
_You can use the ```git reset --hard [fileName]``` to recovery some file that You deleted by a mistake._

____
## Part 5 - More help:
Please visit [GitHub Docs](https://docs.github.com/en) to learn everithing else do You want about _"using git/GitHub"_.