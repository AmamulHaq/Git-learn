## Git
Git is a version control system. [Download Git](https://git-scm.com/downloads) <br>
1: save your Projects/Folders in local (offline).<br>
2: tracking commits and changes over time.<br>
3: parallel working on branches and merging them.

## Github
Github is a web-platform used for hosting your Projects.[Web_Github](https://github.com/)<br>
1: create online repository and push your projects.<br>
2: clone others repository and collaborative project.<br>
3: contribute to open source, fork others project. 

## Git Commands
|S.N |For/To |Commands|Comments|
|---|---|---|---|
|1|Git setup (offline) |git config --global user.name &lt;username&gt;|your git and github with same username |
|||git config --global user.email &lt;email&gt;|your git and github with same email|
||Check setup|git config --list|To check if entered username and email is of single account or not|
|2|Project setup|cd&lt;local path&gt;|go to working space/path/folder|
|||mkdir&lt;project name&gt;|create folder/project name|
|||cd&lt;project name&gt;|go to working project |
|3|Git initialization|git init|initialize git features in local|
|4|Project start|touch&lt;filename&gt;<br>code&lt;filename&gt;|create file and nested folder using VS code|
|5|Git add and commit to save project|git status<br>git add&lt;files/folders&gt;<br> OR git add .|save the changes in files and projects time to time |
|||git commit -m "changes made"|git commit for tracking the activity|
|||git commit -a "deleted file"|just to reflect the changes after deletion of file |
|6|Git workflow|git log|to check the history of commits|
|||git checkout &lt;commit hash&gt;|go to previous commit with in git log activity|
|7|Branch create and work on it|git branch &lt;new branch&gt;<br>git branch -d &lt;deletebranch&gt;|to create new branch and to delete that branch|
|||git branch -a <br> git checkout &lt;branch name&gt;|to check all branches and work on that branch|
|||git checkout -b &lt;branch name&gt;|direct create and switch to work on that branch|
|||git touch &lt;file&gt;<br>code &lt;file&gt;<br>git add &lt;file&gt;<br>git commit -m "changes made"|workflow on that branch|
|8|Back tracking|git reset &lt;commit hash&gt;<br>git reset --hard &lt;commit hash&gt;|undo last commit OR go to previous correct git log activity (delete next commits)|
|||git checkout -b &lt;new-branch-name&gt; &lt;commit hash&gt;|to work in new branch from correct git commit |
|9|Solve merge conflicts|git stash <br>git checkout &lt;main/master&gt;<br>git merge &lt;branch name&gt;|stash saves local changes and merge that branch with main/master and resolve it manually|

<br>

## Github Commands
|S.N |For/To |Commands|Comments|
|---|---|---|---|
|1|Create github repository|[signup](https://github.com/)|login and create online repository|
||go to the project folder|cd &lt;project path&gt;|go to project path to link|
|2|link github repository|git remote add origin &lt;SSH url&gt;|link the online repository with your local project|
||to check the repsitory|git remote -v|valid working in that repository in main|
|3|Project start|touch &lt;filename&gt; <br> code&lt;filename&gt;|work on project locally|
|4|Project activity log|git status<br> git add .<br> git commit -m "changes made"<br>git commit -a "deleted file"|push your project in local git offline|
||to check repo activity|git log --oneline| to inspect recent commit history|
|5|push project in repository|git push origin main|link the project to online repository|
|6|github branch|git branch &lt;branch name&gt;<br>git branch -a|to create and show all branches|
|7|fetch all branches|git fetch --all<br> OR git pull origin main|fetch all branches from github which was worked before|
|8|merge the branches|git merge &lt;branch name&gt;|solve merge conflict and merge in main|
<br>

## Clone project
|S.N |For/To |Commands|Comments|
|---|---|---|---|
|1|To work on others repo go to that repo and copy SSH url||other online repo to own local project|
|2|Clone repo|git clone &lt;SSH url&gt;|clone the repo in local and link it with project|
<br>

## fork and pull request
|S.N|For/To |Commands|Comments|
|---|---|---|---|
|1|contribute to other projects just go to others repo and fork it in to your repo||copy other online repo to own online repo|
|2|Clone fork repo|git clone &lt;SSH url&gt;|clone the fork repo in local and work on it|
<br>

## miscellaneous
|S.N|For/To |Commands|Comments|
|---|---|---|---|
|1|rename master to main|git branch -m master main||
|2|to deatach the committed file |git rm --cached &lt;file name&gt;|use it to reflect the git ingore of that file in repository|
|3|create git ignore |touch .gitignore <br> code .gitignore <br>|/node_modules/, .env,API, passwords|
|4|to ignore the file|&lt;filename&gt; ignore all files of same name <br> /cd/&lt;filename&gt;/ to ignore respective file|git ignore can be nested|
|5|<type>(optional scope): sort in present tense<br> long summary in past tense |git commit -m "feat: add button feature"|use -m in between different commits|
|LAST|git fetch --all|git pull --rebase|git push --force origin main|
<br>