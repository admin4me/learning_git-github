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
git log <p> show all commits in the current branch's history </p>
<h1> Share & Update <h1>
git remote add [alias] [url] <p> used to add an initiated git directory from your local system to a remote system. alias can be anything generally it is origin. url will be from a blank repository created in github.</p><br>
git fetch [alias] <p>fetch down all the branches from that git remote</p><br>
git merge [alias]/[branch] <p> merge a remote branch into your current branch to bring it up to date </p><br>
git push [alias] [branch] <p> transmit local branch commits to the remote repository branch </p><br>
git pull <p> fetch and merge any commits from the tracking remote branch