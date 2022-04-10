### Git Commands
 

#### git config --global user.name 'Syed Shujaat' ==> To set the username Like if anyone see our profile he will see this username

#### git config --global user.email shujaatalibukhari786@gmail.com ==> setting the Email


### To check whether the email and user name are set or not
#### git config --global user.email
#### git config --global user.name


#### git init ==> initailize the empty repository in the current location
#### git add README.md 
#### git commit -m "first commit"  

#### git status ==> to check the status of the git repo

#### git status -s ==> to check the summary status of the git repo

### if it shows untracked files means the file is not staged on the git repo. means git is not taking care of our file
### so to put our files into git we write

#### git add filename ==>  it will add the file to stage portion means in git repo now we can commit it on our local repo and then
#### send it to the remote repository (github).

#### red color means not staged 
#### green color means it is staged and now you can commit

#### git clone url ==> copy a project from given url

#### git commit -m "Commit message" this will commit the staged file

#### touch about.html ==> This will create a html file

#### git add -A ==> add all the files to staging area.

#### git checkout contact.html ==> undo all the changes of file contact.html upto the last commit
#### git checkout -f ==> undo all the changes of all the files upto last commit


#### git log ==> this will show you how many commits you have done so far

### If we have 1000 commits and we want to see only a most recent five then 

#### git log -p -5

#### git diff ==> to show the difference between working area and stage area

#### git diff --staged ==> show the difference between the commited and staged area

#### git commit -a -m "Commit all without staging" ==> this will commit all the files by skipping the staging them (We should avoid this becase
#### it is not a professional approach to do things)

#### git rm --cached filename ==> (If mistakenly we staged and commited a file now we want to remove it from git repo but we want it on 
#### our hard drive then we use this)

#### git rm filename ==>(This will remove the file evern from repo and harddrive)

-----------------------------------------------------------------------------
### Git Branching

#### git branch  ==> To check in which branch i am 

#### git branch feature1 ==> create a branch with named features

#### git checkout feature1 ==> moved to feature1 branch

#### git checkout -b Mybranch ==> This will create and switch you to new created branch in one go

#### remove a branch locally ==> git branch -d feature1

### To merge the changes of branch we switch to the master branch first where we want to merge the changes then we write
#### git merge feature1

### Adding the local repo to github  

#### git remote add origin url

#### git push origin master

#### git push -u origin master ==> To push the master branch into the github

#### git push -u origin feature1 ==> ( If we use -u It will select that particular branch) Next Time when we push It we don't need to specify branch
#### git push ==> It will push to feature1 branch now because It is selected in the above command

#### git push feature1 ( If we have not used -u every time we have to specify branch name in which we want to push the code)

#### git pull origin master ( fetch the code from the remote repo)

#### git pull -u origin master (pull the code and select the master branch now whenever we say git pull by default master branch is selected)
#### git pull -> No need to write branch now





