# GitTestt

Hello, everyone, this is a demo project for learning git and github

To install git:

download and install git bash: https://git-scm.com
--------------------


#Git Commands:

1) check git version: git --version
2) git init : initiallizing git
3) create file touch command : touch filename
4) by adding file for stageing area, so git trekk the file: git add filename, git add . and git add -A
5) commit for save it git commit -m "message"
6) check it is in staging area or not: git status
7) git rm --cached filename(taking out of trekking), rm filename.
8) (check or commits current branch):git log
9) making branch: git branch branchname
10) (to switch in branch): git checkout branchname
11) (creating new branch and switch in that branch):git checkout -b branchname 
12) check branches in project: git branch -> shows *branchname(current branch opened) all branches
13) Merge branch in parent branch or master branch: git merge branchname
14) grapg of all branches: git log --all 

#Connect git to github:

Connect git repository to github:
1) two ways: https or ssh
1.1) through https: git remote add origin "https://github.com/user/repo.git"
1.2) through ssh: git remote add ssh-origin "git@github.com:user/hello-world.git"
2) changing remote origin from https to ssh: git remote set-url remote-name git@github.com:username/repositor.git
3) Push repo to github: git push origin master or git push --set-upstream origin master or git push ssh-origin url
4) checking which branch added/connected to remote: git branch -r
5) pull changes on remote: git pull origin master
6) create new branch and switch in that branch: git checkout -b branchname


#Commands to create ssh keys step by step:

1) ssh keygen
2) cd ~/.ssh (~for root)
3) ls(shows all files)
4) to check id(encrypted id): cat id_rsa.pub
5) pwd(check current path)
6) add agent which manage id both public as well private: eval 'ssh-agent'
7) shows id added: ssh-add ~ /.ssha/id_rsa
8) ssh add -l
9) (authicated or not shows username-github):ssh -T git@github.com


#.gitignore
add files, which you don't want upload
1) filename.extension (to ignore single file)
2) *.temp(to ignore all files which has .temp extension)

#Git Stash Commands
1) save last changes when work is not done without commit after adding file or branch in staging area then type: git stash
2) save last changes to file or branch use putting in stash for proper with message so, easily be identified: git stash push -m "updated in file1.txt"
3) apply last changes which is in stash: stash apply
4) remove stash single entry from stash list: git stash drop 1
5) for add changes to file and delete file from stash: git stash pop 1
6) to show all stash list: git stash list
7) clean all stash list: git clean or git clean





