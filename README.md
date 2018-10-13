**touch index.html**\
touch command is to create a file, in this case create an index.html file.

then\
**git init**\
this initializes a git repository

then to add our user name\
**git config --global user.name 'vasudevapitta'**

then to add our email\
**git config --global user.email 'tizzicboy@gmail.com'**

then to add index.html to the git repository\
**git add index.html**

then if we want to check whether index.html is added to the staging area, we can do\
**git status**

then if we want to remove index.html file from the staging area we can do\
**git rm --cached index.html**

then if we want to add all the files to the staging area we can do\
**git add .**

then if we want to commit the staging area (for the first time per project) then we can do\
**git commit**\
and then hit i to enter into insert mode and then we can type our commit message and hit escape to get out of insert mode\
and then type **:wq **and hit enter\

now if we make more changes in our files we can do\
**git add .**\
to add the files to the staging area\
then to commit the changes we can do\
**git commit -m 'your commit message'**\
this will skip the process of entering into insert mode and then writing our commit message and then hitting escape and then typing :wq and hitting enter

to clear everything\
**clear**

to create gitignore file\
**touch .gitignore**\
then open your .gitignore file in text editor and add the file name which you want to be ignored

branch master is the master branch or the Main project\
to get your own copy of the main project you need to branch it by\
**git branch nameOfTheBranch**

now to get into the newly created branch we do\
**git checkout nameOfTheBranch**

to switch back into the master branch\
**git checkout master**\
every time we switch the branch we will see different versions of our files with the changes we made while we are in that branch

to merge a newly created branch with the master branch\
**git checkout master **(to be on the master branch) then\
**git merge login **(and hit enter) then hit i for insert mode and then enter your commit message and then hit **escape and then type :wq **and hit enter\
this adds all the files created on the newlyCreatedBranch into the master branch

**git remote**\
to see if there are any remote repositories

go to github create a new repository with a name and copy the remote url into git bash and hit enter\
**git remote add origin https://github.com/vasudevapitta/nameOfTheRepo.git**

then copy\
**git push -u origin master**\
into git bash and hit enter\
if prompted from your windows machine login with your github credentials (username & password)

every time after we make any changes locally on our machine we do\
**git push**\
to push the project into the remote repository

to clone a project copy the url from github\
cd into your new directory and open git bash there\
**git clone https://github.com/vasudevapitta/nameOfTheRepo.git**\

If other developers made changes in your repo and you want to pull the project into your local machine\
**git pull**