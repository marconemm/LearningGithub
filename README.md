# Repository to learn Github

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
2. ### Fetching: <br>
   _Now You need to synchronize your local repo with the origin repo. To to it, use the command ```"fetch"```_.
   1.  ```git fecth origin```
3. ### Pushing: <br>
   _Now You're able to send your 1st commit to the ```"origin"``` (the remote repo)_.
   1.  ```git push origin master ``` _(or the ```BranchName``` that You could be working on)_```_