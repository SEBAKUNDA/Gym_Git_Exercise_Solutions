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

#bundle 1
exercise2

```bash
Eric-2:Gym_Git_Exercise_Solutions mac$ stash list
bash: stash: command not found
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash list
stash@{0}: WIP on main: b1a4408 defhf
stash@{1}: WIP on main: b1a4408 defhf
stash@{2}: WIP on main: b1a4408 defhf
stash@{3}: WIP on main: b1a4408 defhf
stash@{4}: WIP on main: b1a4408 defhf
stash@{5}: WIP on main: b1a4408 defhf
stash@{6}: WIP on main: b1a4408 defhf
stash@{7}: WIP on main: b1a4408 defhf
stash@{8}: WIP on main: b1a4408 defhf
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0} 
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   home.html
        new file:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        home.

Dropped stash@{0} (345a88fa8c509301b794113a84a1a9d4c16a7c4e)
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash list
stash@{0}: WIP on main: b1a4408 defhf
stash@{1}: WIP on main: b1a4408 defhf
stash@{2}: WIP on main: b1a4408 defhf
stash@{3}: WIP on main: b1a4408 defhf
stash@{4}: WIP on main: b1a4408 defhf
stash@{5}: WIP on main: b1a4408 defhf
stash@{6}: WIP on main: b1a4408 defhf
stash@{7}: WIP on main: b1a4408 defhf
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0} 
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   about.html
        new file:   home.html
        new file:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        home.

Dropped stash@{0} (f409dcff1f2bffe52a2c39dbff4887f47abbff03)
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0} 
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash list
stash@{0}: WIP on main: b1a4408 defhf
stash@{1}: WIP on main: b1a4408 defhf
stash@{2}: WIP on main: b1a4408 defhf
stash@{3}: WIP on main: b1a4408 defhf
stash@{4}: WIP on main: b1a4408 defhf
stash@{5}: WIP on main: b1a4408 defhf
stash@{6}: WIP on main: b1a4408 defhf
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0} 
home.html: needs merge
unable to refresh index
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{1}
home.html: needs merge
unable to refresh index
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{1}
home.html: needs merge
unable to refresh index
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
home.html: needs merge
unable to refresh index
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash list
stash@{0}: WIP on main: b1a4408 defhf
stash@{1}: WIP on main: b1a4408 defhf
stash@{2}: WIP on main: b1a4408 defhf
stash@{3}: WIP on main: b1a4408 defhf
stash@{4}: WIP on main: b1a4408 defhf
stash@{5}: WIP on main: b1a4408 defhf
stash@{6}: WIP on main: b1a4408 defhf
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{6}
home.html: needs merge
unable to refresh index
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
home.html: needs merge
unable to refresh index
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop
home.html: needs merge
unable to refresh index
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash list
stash@{0}: WIP on main: b1a4408 defhf
stash@{1}: WIP on main: b1a4408 defhf
stash@{2}: WIP on main: b1a4408 defhf
stash@{3}: WIP on main: b1a4408 defhf
stash@{4}: WIP on main: b1a4408 defhf
stash@{5}: WIP on main: b1a4408 defhf
stash@{6}: WIP on main: b1a4408 defhf
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        new file:   about.html
        new file:   home.
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (70bb423ff66f9304781fe0d1479018e7e26e7bd4)
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash list
stash@{0}: WIP on main: b1a4408 defhf
stash@{1}: WIP on main: b1a4408 defhf
stash@{2}: WIP on main: b1a4408 defhf
stash@{3}: WIP on main: b1a4408 defhf
stash@{4}: WIP on main: b1a4408 defhf
stash@{5}: WIP on main: b1a4408 defhf
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        new file:   about.html
        new file:   home.
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (ef3e37fa0de07da6927764f6cb30afc14e6e39b9)
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
Auto-merging about.html
CONFLICT (add/add): Merge conflict in about.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        new file:   about.html
        new file:   home.
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (979c6579b1dd0f5e719da82c69c452386506e39b)
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
Auto-merging about.html
CONFLICT (add/add): Merge conflict in about.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        new file:   about.html
        new file:   home.
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (73d48a47f365107c0e428a9273e17aac7efb01a8)
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        new file:   about.html
        new file:   home.
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (00b1032329022b65dc7556f275b55f804a5ad254)
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
Auto-merging about.html
CONFLICT (add/add): Merge conflict in about.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        new file:   about.html
        new file:   home.
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (2f5a1fc035f3cb7afcf7d4d0372dabf5e39f0f45)
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
        new file:   about.html
        new file:   home.
        new file:   home.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash
Saved working directory and index state WIP on main: c9ba7f1 starting exercise 2
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash
Saved working directory and index state WIP on main: c9ba7f1 starting exercise 2
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash
Saved working directory and index state WIP on main: c9ba7f1 starting exercise 2
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash list
stash@{0}: WIP on main: c9ba7f1 starting exercise 2
stash@{1}: WIP on main: c9ba7f1 starting exercise 2
stash@{2}: WIP on main: c9ba7f1 starting exercise 2
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   about.html

Dropped stash@{1} (9d8eaa243005993ca52e7f2c4ff82cfd97773b63)
Eric-2:Gym_Git_Exercise_Solutions mac$  git stash list
stash@{0}: WIP on main: c9ba7f1 starting exercise 2
stash@{1}: WIP on main: c9ba7f1 starting exercise 2
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   about.html
        new file:   home.html

Dropped stash@{1} (11f6c68408c0dcaa6646be22a8e0f18cba7290ff)
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"second commit"
[main af3a4c1] second commit
 2 files changed, 24 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
Counting objects: 4, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 537 bytes | 268.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   c9ba7f1..af3a4c1  main -> main
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash list
stash@{0}: WIP on main: c9ba7f1 starting exercise 2
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   team.html

Dropped stash@{0} (b6441a1161faff2b9a2969dc0d537e0b5b2d55ce)
Eric-2:Gym_Git_Exercise_Solutions mac$  git reset --hard
HEAD is now at af3a4c1 second commit
Eric-2:Gym_Git_Exercise_Solutions mac$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
Eric-2:Gym_Git_Exercise_Solutions mac$ 

```
#bundle2

#Exercise1

```bash
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout ft/bundle-2
swiched to ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        service.html

nothing added to commit but untracked files present (use "git add" to track)
Eric-2:Gym_Git_Exercise_Solutions mac$  git add  service.html
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"service commit"
[main a2c67ce] service commit
 1 file changed, 12 insertions(+)
 create mode 100644 service.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 472 bytes | 472.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   7fbcc5f..a2c67ce  main -> main
```
#bundle2
#Exercise2
```bash
Eric-2:Gym_Git_Exercise_Solutions mac$  git checkout -b ft/service-redesign
M       README.md
Switched to a new branch 'ft/service-redesign'
    git push --set-upstream origin ft/service-redesign

Eric-2:Gym_Git_Exercise_Solutions mac$ git push --set-upstream origin ft/service-redesign
fatal: unable to access 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git/': Operation timed out after 300013 milliseconds with 0 out of 0 bytes received
Eric-2:Gym_Git_Exercise_Solutions mac$ git push --set-upstream origin ft/service-redesign
Counting objects: 6, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 781 bytes | 781.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   7f5ac6f..f5076c0  ft/service-redesign -> ft/service-redesign
Branch 'ft/service-redesign' set up to track remote branch 'ft/service-redesign' from 'origin'.
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   services.html

Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"change after pull request"
[main 9a0d427] change after pull request
 1 file changed, 2 insertions(+), 4 deletions(-)
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
fatal: unable to access 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git/': Could not resolve host: github.com
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
fatal: unable to access 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git/': Could not resolve host: github.com
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
fatal: unable to access 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git/': Could not resolve host: github.com
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
fatal: unable to access 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git/': Could not resolve host: github.com

Eric-2:Gym_Git_Exercise_Solutions mac$  git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), done.
From https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions
   03af281..4491fa1  main       -> origin/main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.


Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit - m"changes"

Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 5 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:

        modified:   service.html
        modified:   services.html

Eric-2:Gym_Git_Exercise_Solutions mac$  git add services.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"services"
[main c3591b4] services


Eric-2:Gym_Git_Exercise_Solutions mac$ git push
Counting objects: 6, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 633 bytes | 18.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   4491fa1..c3591b4  main -> main

Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.


Eric-2:Gym_Git_Exercise_Solutions mac$   git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.


Eric-2:Gym_Git_Exercise_Solutions mac$  git merge main
Already up to date.
Eric-2:Gym_Git_Exercise_Solutions mac$  git checkout -b ft/service-redesign
fatal: A branch named 'ft/service-redesign' already exists.
Eric-2:Gym_Git_Exercise_Solutions mac$  git branch -d ft/service-redesign
Deleted branch ft/service-redesign (was f5076c0).
Eric-2:Gym_Git_Exercise_Solutions mac$  git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

Eric-2:Gym_Git_Exercise_Solutions mac$  git add modified:   services.html
fatal: pathspec 'modified:' did not match any files
Eric-2:Gym_Git_Exercise_Solutions mac$  git add   services.html
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"commiting services again"
[ft/service-redesign fbcae1f] commiting services again
 1 file changed, 3 insertions(+), 2 deletions(-)
Eric-2:Gym_Git_Exercise_Solutions mac$  git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

Eric-2:Gym_Git_Exercise_Solutions mac$  git push --set-upstream origin ft/service-redesign
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 309 bytes | 309.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   f5076c0..fbcae1f  ft/service-redesign -> ft/service-redesign
Branch 'ft/service-redesign' set up to track remote branch 'ft/service-redesign' from 'origin'.
Eric-2:Gym_Git_Exercise_Solutions mac$  git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
Eric-2:Gym_Git_Exercise_Solutions mac$  git add services.html
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m" services in main"
[main 737aa73]  services in main
 1 file changed, 2 insertions(+), 4 deletions(-)
Eric-2:Gym_Git_Exercise_Solutions mac$  git push
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Eric-2:Gym_Git_Exercise_Solutions mac$  git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), done.
From https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions
   c3591b4..0e5875a  main       -> origin/main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
Eric-2:Gym_Git_Exercise_Solutions mac$  git merge 
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
Eric-2:Gym_Git_Exercise_Solutions mac$  git push
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Eric-2:Gym_Git_Exercise_Solutions mac$  git push
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Eric-2:Gym_Git_Exercise_Solutions mac$ git merge main
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
Eric-2:Gym_Git_Exercise_Solutions mac$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 2 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:

        modified:   services.html

Eric-2:Gym_Git_Exercise_Solutions mac$  git add services.html
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"before merge"
[main 728c303] before merge
Eric-2:Gym_Git_Exercise_Solutions mac$  git push
Counting objects: 6, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 670 bytes | 670.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   0e5875a..728c303  main -> main
Eric-2:Gym_Git_Exercise_Solutions mac$  git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
Eric-2:Gym_Git_Exercise_Solutions mac$  git merge main
Updating fbcae1f..728c303
Fast-forward
 services.html | 1 +
 1 file changed, 1 insertion(+)
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch ft/service-redesign
Your branch is ahead of 'origin/ft/service-redesign' by 3 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
Eric-2:Gym_Git_Exercise_Solutions mac$  git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
Eric-2:Gym_Git_Exercise_Solutions mac$  git branch checkout ft/service-redesign
fatal: A branch named 'checkout' already exists.
Eric-2:Gym_Git_Exercise_Solutions mac$  git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is ahead of 'origin/ft/service-redesign' by 3 commits.
  (use "git push" to publish your local commits)
Eric-2:Gym_Git_Exercise_Solutions mac$  git giff main
git: 'giff' is not a git command. See 'git --help'.

The most similar command is
        diff
Eric-2:Gym_Git_Exercise_Solutions mac$ git diff main
Eric-2:Gym_Git_Exercise_Solutions mac$  git diff main
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Eric-2:Gym_Git_Exercise_Solutions mac$  git merge ft/service-redesign
Already up to date.
```
