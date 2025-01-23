# learning_git-github
I am going to write commands for git integration in system <br>
github is free code hosting platform. where you can even save your private or public code<br>
after installing git in your windows open terminal to configure your credential in git <br>
during code to open your terminal in vscode press ctrl+shift+~<br><br>
<h1> Setup </h1>
git --version <p>this command is used to check version of git installed in your system</p><br>
git config --global user.name "give your username in quotation" </p>this is used to configure your username in git<p><br>
git config --list <p> list user credentials </p><br>
git config --global user.email "valid email in quotation" <p> this is used to add email </p><br>
<h1> Setup & Init </h1>
git clone url of your code on github <p> this is used to bring your repository from github to your local sysem. you can even bring anyone's code using link.</p><br>
git init <p> make your current working directory a git directory for using git command. </p><br>
<p> the file will be cloned in same directory where your git is installed open the using ctrl+k+o </p> <br>
<h1> Stag and Snapshot </h1>
git status <p>show modified files in in working directory, staged for your next commit. </p><br>
git add filename <p>stag a file for your next commit, you can use (git add .) without bracket to stage changes in all files <p><br>
git reset filename <p>unstage a file while retaining working directory </p>
git diff <p>shows difference of what is changed but not staged </p><br>
git diff --staged <p> difference of what is staged but not yet commited </p><br>
git commit -m "commint messege in quotation" <p> commit your staged changes with the commit messege</p><br>
<h1> Branch & Merge </h1>
git branch <p> list your branches. a* will appear next to current active branch. </p><br>
git branch [branch-name] <p> create a new branch at the current commit </p><br>
git checkout [branch-name] <p> swithch to another branch and check it out into your working directory </p>
git merge [branch] <p> merge the specified branch's history with the current one </p><br>
git branch -M [new branch name] <p> used to change the branch name of your current branch </p><br>
git branch -d [branch name] <p>used for deleting a branch except your current one. </p><br>
git diff [branch name] <p> to compare commits between branches, files and more</p><br>
<p>An another to method to merge is create pull requst for merge using github. which is used in industries </p><br>
git log <p> show all commits in the current branch's history. press q to quit from log </p>
<h1> Share & Update </h1>
git remote add [alias] [url] <p> used to add an initiated git directory from your local system to a remote system. alias can be anything generally it is origin. url will be from a blank repository created in github.</p><br>
git remote -v <p> To verify remote </p><br>
git fetch [alias] <p>fetch down all the branches from that git remote</p><br>
git merge [alias]/[branch] <p> merge a remote branch into your current branch to bring it up to date </p><br>
git push [alias] [branch] <p> transmit local branch commits to the remote repository branch </p><br>
git push -u [alias] [branch] <p> -u will save your default alias and branch next you press git push it will take alias and branch without saying.<br>
git pull <p> fetch and merge any commits from the tracking remote branch you can add alias and branch as well.</p><br>
<h1> Rewrite History </h1>
git reset [file name] <p>This command is used to reset from staged but not commited.<p><br>
git reset HEAD~1 <p> This can be used to go back for 1 commit. </p><br>
git reset [commit hash] <p> This will directly move back to that commit. has of commit can be found in log </p><br>
git reset --hard [commit has] <p> this will move back to that commit and the code in vs code will also roll back at that commit, while in above the vs code retain it's codes</p><br>
