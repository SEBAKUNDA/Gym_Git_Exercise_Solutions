# Gym_Git_Exercise_Solutions
# git exercise

#bundle 1

#exercise 1

```bash
Eric-2:git--exercise mac$ git init
Initialized empty Git repository in /Users/mac/git--exercise/.git/
Eric-2:git--exercise mac$  git branch -m master main
error: refname refs/heads/master not found
fatal: Branch rename failed
Eric-2:git--exercise mac$ git add .
Eric-2:git--exercise mac$ git commit -m "first commit"
[master (root-commit) d53bb28] first commit
 2 files changed, 12 insertions(+)
 create mode 100644 README.md
 create mode 100644 indexx.html
Eric-2:git--exercise mac$ git remote add origin https://github.com/SEBAKUNDA/git.git
Eric-2:git--exercise mac$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

Eric-2:git--exercise mac$  git push --set-upstream origin master
Counting objects: 4, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 447 bytes | 24.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/SEBAKUNDA/git.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
Eric-2:git--exercise mac$ 
```
