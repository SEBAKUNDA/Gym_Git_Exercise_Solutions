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
#bundle4
# exercise1
```bash
Eric-2:Gym_Git_Exercise_Solutions mac$ git branch
  ft/bundle-2
  ft/contact-page
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 6 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)
Eric-2:Gym_Git_Exercise_Solutions mac$ git remote add git-copy https://github.com/exampleuser/git-copy-repo.git

Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"changes on question 4"
[main 707741c] changes on question 4
 1 file changed, 2 insertions(+), 2 deletions(-)





Eric-2:Gym_Git_Exercise_Solutions mac$ git remote -v
git-copy        https://github.com/exampleuser/git-copy-repo.git (fetch)
git-copy        https://github.com/exampleuser/git-copy-repo.git (push)
origin  https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git (fetch)
origin  https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git (push)


Eric-2:Gym_Git_Exercise_Solutions mac$ git remote add git-copy https://github.com/SEBAKUNDA/New_changes.git
fatal: remote git-copy already exists.


Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"commmit"
[main 3dcaf4f] commmit
 1 file changed, 1 insertion(+), 1 deletion(-)







Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"git"
\[main 9de3abe] git
Eric-2:Gym_Git_Exercise_Solutions mac$  git pull origin main
From https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.
Eric-2:Gym_Git_Exercise_Solutions mac$  git push origin main
Counting objects: 13, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (13/13), done.
Writing objects: 100% (13/13), 1.25 KiB | 638.00 KiB/s, done.
Total 13 (delta 8), reused 0 (delta 0)
remote: Resolving deltas: 100% (8/8), completed with 4 local objects.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   9abe8a7..9de3abe  main -> main
Eric-2:Gym_Git_Exercise_Solutions mac$ git remote add git-copy https://github.com/exampleuser/git-copy-repo.git
fatal: remote git-copy already exists.
Eric-2:Gym_Git_Exercise_Solutions mac$  cd https://github.com/SEBAKUNDA/New_changes.git
bash: cd: https://github.com/SEBAKUNDA/New_changes.git: No such file or directory
Eric-2:Gym_Git_Exercise_Solutions mac$ git branch
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
  ft/team-page
* main
  remotes
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout -b git-copy
Switched to a new branch 'git-copy'

Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"committ"
[git-copy 80e2b6e] committ
 1 file changed, 1 insertion(+), 1 deletion(-)

Eric-2:Gym_Git_Exercise_Solutions mac$   git push --set-upstream origin git-copy
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 285 bytes | 285.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'git-copy' on GitHub by visiting:
remote:      https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions/pull/new/git-copy
remote: 
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 * [new branch]      git-copy -> git-copy
Branch 'git-copy' set up to track remote branch 'git-copy' from 'origin'.
Eric-2:Gym_Git_Exercise_Solutions mac$ c
```
#bundle4
#exercise2

```bash
Eric-2:Gym_Git_Exercise_Solutions mac$ git branch
  ft/bundle-2
  ft/contact-page
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 6 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)
Eric-2:Gym_Git_Exercise_Solutions mac$ git remote add git-copy https://github.com/exampleuser/git-copy-repo.git
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 6 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"changes on question 4"
[main 707741c] changes on question 4
 1 file changed, 2 insertions(+), 2 deletions(-)
Eric-2:Gym_Git_Exercise_Solutions mac$  git push git-copy main origin main
error: src refspec origin does not match any.
error: failed to push some refs to 'https://github.com/exampleuser/git-copy-repo.git'
Eric-2:Gym_Git_Exercise_Solutions mac$ git push origin master git-copy master
error: src refspec master does not match any.
error: src refspec git-copy does not match any.
error: src refspec master does not match any.
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
Eric-2:Gym_Git_Exercise_Solutions mac$ git push origin main git-copy main
error: src refspec git-copy does not match any.
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
Eric-2:Gym_Git_Exercise_Solutions mac$ git add remote https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
fatal: pathspec 'remote' did not match any files
Eric-2:Gym_Git_Exercise_Solutions mac$ git push --all
Counting objects: 7, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 5.07 KiB | 2.53 MiB/s, done.
Total 7 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   fbcae1f..8289711  ft/service-redesign -> ft/service-redesign
 * [new branch]      remotes -> remotes
 ! [rejected]        ft/bundle-2 -> ft/bundle-2 (non-fast-forward)
 ! [rejected]        ft/team-page -> ft/team-page (non-fast-forward)
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Eric-2:Gym_Git_Exercise_Solutions mac$ git push --all origin git-copy
error: --all can't be combined with refspecs
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --repo <repository>   repository
    --all                 push all refs
    --mirror              mirror all refs
    -d, --delete          delete refs
    --tags                push tags (can't be used with --all or --mirror)
    -n, --dry-run         dry run
    --porcelain           machine-readable output
    -f, --force           force updates
    --force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --recurse-submodules[=<check|on-demand|no>]
                          control recursive pushing of submodules
    --thin                use thin pack
    --receive-pack <receive-pack>
                          receive pack program
    --exec <receive-pack>
                          receive pack program
    -u, --set-upstream    set upstream for git pull/status
    --progress            force progress reporting
    --prune               prune locally removed refs
    --no-verify           bypass pre-push hook
    --follow-tags         push missing but relevant tags
    --signed[=<yes|no|if-asked>]
                          GPG sign the push
    --atomic              request atomic transaction on remote side
    -o, --push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only

Eric-2:Gym_Git_Exercise_Solutions mac$ git push --all origin git-copy
error: --all can't be combined with refspecs
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --repo <repository>   repository
    --all                 push all refs
    --mirror              mirror all refs
    -d, --delete          delete refs
    --tags                push tags (can't be used with --all or --mirror)
    -n, --dry-run         dry run
    --porcelain           machine-readable output
    -f, --force           force updates
    --force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --recurse-submodules[=<check|on-demand|no>]
                          control recursive pushing of submodules
    --thin                use thin pack
    --receive-pack <receive-pack>
                          receive pack program
    --exec <receive-pack>
                          receive pack program
    -u, --set-upstream    set upstream for git pull/status
    --progress            force progress reporting
    --prune               prune locally removed refs
    --no-verify           bypass pre-push hook
    --follow-tags         push missing but relevant tags
    --signed[=<yes|no|if-asked>]
                          GPG sign the push
    --atomic              request atomic transaction on remote side
    -o, --push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only

Eric-2:Gym_Git_Exercise_Solutions mac$  git push . origin it-copy
error: src refspec origin does not match any.
error: src refspec it-copy does not match any.
error: failed to push some refs to '.'
Eric-2:Gym_Git_Exercise_Solutions mac$  git push . origin git-copy
error: src refspec origin does not match any.
error: src refspec git-copy does not match any.
error: failed to push some refs to '.'
Eric-2:Gym_Git_Exercise_Solutions mac$  git push . origin main  git-copy main
error: src refspec origin does not match any.
error: src refspec git-copy does not match any.
error: failed to push some refs to '.'
Eric-2:Gym_Git_Exercise_Solutions mac$  git push origin main git-copy main
error: src refspec git-copy does not match any.
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
Eric-2:Gym_Git_Exercise_Solutions mac$  git push origin main git-copy main
error: src refspec git-copy does not match any.
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
Eric-2:Gym_Git_Exercise_Solutions mac$  git branch
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
  ft/team-page
* main
  remotes
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch main
Your branch and 'origin/main' have diverged,
and have 2 and 6 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean
Eric-2:Gym_Git_Exercise_Solutions mac$ git remote -v
git-copy        https://github.com/exampleuser/git-copy-repo.git (fetch)
git-copy        https://github.com/exampleuser/git-copy-repo.git (push)
origin  https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git (fetch)
origin  https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git (push)
Eric-2:Gym_Git_Exercise_Solutions mac$  git push git remote -v main git-copy main
Pushing to git
error: src refspec remote does not match any.
error: src refspec git-copy does not match any.
error: failed to push some refs to 'git'
Eric-2:Gym_Git_Exercise_Solutions mac$  git push Gym_Git_Exercise_Solutions  main git-copy main
error: src refspec git-copy does not match any.
error: failed to push some refs to 'Gym_Git_Exercise_Solutions'
Eric-2:Gym_Git_Exercise_Solutions mac$ git remote add git-copy https://github.com/SEBAKUNDA/New_changes.git
fatal: remote git-copy already exists.
Eric-2:Gym_Git_Exercise_Solutions mac$ git remote -v
git-copy        https://github.com/exampleuser/git-copy-repo.git (fetch)
git-copy        https://github.com/exampleuser/git-copy-repo.git (push)
origin  https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git (fetch)
origin  https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git (push)
Eric-2:Gym_Git_Exercise_Solutions mac$ git push origin main
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Eric-2:Gym_Git_Exercise_Solutions mac$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 2 and 6 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean
Eric-2:Gym_Git_Exercise_Solutions mac$ git push git-copy -u main
remote: Repository not found.
fatal: repository 'https://github.com/exampleuser/git-copy-repo.git/' not found
Eric-2:Gym_Git_Exercise_Solutions mac$ git remote -v
git-copy        https://github.com/exampleuser/git-copy-repo.git (fetch)
git-copy        https://github.com/exampleuser/git-copy-repo.git (push)
origin  https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git (fetch)
origin  https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git (push)
Eric-2:Gym_Git_Exercise_Solutions mac$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 2 and 6 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"commmit"
[main 3dcaf4f] commmit
 1 file changed, 1 insertion(+), 1 deletion(-)
Eric-2:Gym_Git_Exercise_Solutions mac$  git push origin main
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Eric-2:Gym_Git_Exercise_Solutions mac$ git stash
No local changes to save
Eric-2:Gym_Git_Exercise_Solutions mac$ git pull origin main
From https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions
 * branch            main       -> FETCH_HEAD
error: There was a problem with the editor 'vi'.
Not committing merge; use 'git commit' to complete the merge.
Eric-2:Gym_Git_Exercise_Solutions mac$  git stash pop 
Auto-merging team.html
CONFLICT (content): Merge conflict in team.html
Eric-2:Gym_Git_Exercise_Solutions mac$  git stash
team.html: needs merge
team.html: needs merge
team.html: unmerged (f28b01da1ff329fdce3eee22caec5ba67fe04740)
team.html: unmerged (97bc5fa8a7c9323496b0bc63450f065a3c3f2128)
team.html: unmerged (1c0e1231d04999e5755087c3128c956817e3120e)
fatal: git-write-tree: error building trees
Cannot save the current index state
Eric-2:Gym_Git_Exercise_Solutions mac$  git stash list
stash@{0}: WIP on ft/team-page: 865c8d1 commiting team again
stash@{1}: WIP on ft/team-page: ab63423 ather commit
stash@{2}: WIP on ft/team-page: b6a66a0 next commit
stash@{3}: WIP on ft/team-page: b6a66a0 next commit
stash@{4}: WIP on ft/team-page: 4be818e commit again
Eric-2:Gym_Git_Exercise_Solutions mac$  git push origin main
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Eric-2:Gym_Git_Exercise_Solutions mac$ git pull origin main
error: You have not concluded your merge (MERGE_HEAD exists).
hint: Please, commit your changes before merging.
fatal: Exiting because of unfinished merge.
Eric-2:Gym_Git_Exercise_Solutions mac$ git pull origin main
error: You have not concluded your merge (MERGE_HEAD exists).
hint: Please, commit your changes before merging.
fatal: Exiting because of unfinished merge.
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch main
Your branch and 'origin/main' have diverged,
and have 3 and 6 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:

        new file:   team.html

Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"team"
[main dd0b19d] team
Eric-2:Gym_Git_Exercise_Solutions mac$  git push origin main
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Eric-2:Gym_Git_Exercise_Solutions mac$  git pull origin main
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), done.
From https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions
 * branch            main       -> FETCH_HEAD
   d7ae665..9abe8a7  main       -> origin/main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
Eric-2:Gym_Git_Exercise_Solutions mac$  git pull origin main
error: You have not concluded your merge (MERGE_HEAD exists).
hint: Please, commit your changes before merging.
fatal: Exiting because of unfinished merge.
Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"git"
\[main 9de3abe] git
Eric-2:Gym_Git_Exercise_Solutions mac$  git pull origin main
From https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.
Eric-2:Gym_Git_Exercise_Solutions mac$  git push origin main
Counting objects: 13, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (13/13), done.
Writing objects: 100% (13/13), 1.25 KiB | 638.00 KiB/s, done.
Total 13 (delta 8), reused 0 (delta 0)
remote: Resolving deltas: 100% (8/8), completed with 4 local objects.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   9abe8a7..9de3abe  main -> main
Eric-2:Gym_Git_Exercise_Solutions mac$ git remote add git-copy https://github.com/exampleuser/git-copy-repo.git
fatal: remote git-copy already exists.
Eric-2:Gym_Git_Exercise_Solutions mac$  cd https://github.com/SEBAKUNDA/New_changes.git
bash: cd: https://github.com/SEBAKUNDA/New_changes.git: No such file or directory
Eric-2:Gym_Git_Exercise_Solutions mac$ git branch
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
  ft/team-page
* main
  remotes
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout -b git-copy
Switched to a new branch 'git-copy'
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch git-copy
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"committ"
[git-copy 80e2b6e] committ
 1 file changed, 1 insertion(+), 1 deletion(-)
Eric-2:Gym_Git_Exercise_Solutions mac$  git push 
fatal: The current branch git-copy has no upstream branch.
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch git-copy
Your branch is up to date with 'origin/git-copy'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'
Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"footer"
[ft/footer b787bc3] footer
 1 file changed, 2 insertions(+), 2 deletions(-)
Eric-2:Gym_Git_Exercise_Solutions mac$ git add .
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m"footer again"
[ft/footer 43c437d] footer again
 1 file changed, 1 insertion(+), 1 deletion(-)
Eric-2:Gym_Git_Exercise_Solutions mac$  git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

Eric-2:Gym_Git_Exercise_Solutions mac$ git push --set-upstream origin ft/footer
Counting objects: 6, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 578 bytes | 44.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions/pull/new/ft/footer
remote: 
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
 * [new branch]      ft/footer -> ft/footer
Branch 'ft/footer' set up to track remote branch 'ft/footer' from 'origin'.
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout ft/footer
Switched to branch 'ft/footer'
Your branch is up to date with 'origin/ft/footer'.
Eric-2:Gym_Git_Exercise_Solutions mac$ git merge --squash ft/footer
 (nothing to squash)Already up to date.
Eric-2:Gym_Git_Exercise_Solutions mac$ git merge --squash ft/footer
 (nothing to squash)Already up to date.
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"ooter changes squashing"
On branch ft/footer
Your branch is up to date with 'origin/ft/footer'.

Changes not staged for commit:
        modified:   services.html

no changes added to commit
Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"ooter changes squashing"
[ft/footer 6da135b] ooter changes squashing
 1 file changed, 1 insertion(+), 1 deletion(-)
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   43c437d..6da135b  ft/footer -> ft/footer
Eric-2:Gym_Git_Exercise_Solutions mac$ 
```
#bundle 4
#Exercise2

```bash

Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout -b  ft/footer
Switched to a new branch 'ft/footer'
Eric-2:Gym_Git_Exercise_Solutions mac$  git add  footer.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"commit of footer"
[ft/footer 1a112ba] commit of footer
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git add    footer1.html
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m" footer1"
[ft/footer 79e55e1]  footer1
 1 file changed, 12 insertions(+)
 create mode 100644 footer1.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git status
On branch main
Your branch is behind 'origin/main' by 8 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"commit"
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'
Eric-2:Gym_Git_Exercise_Solutions mac$ git add footer.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"footer"
[ft/footer 05a20fe] footer
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html
Eric-2:Gym_Git_Exercise_Solutions mac$  git add footer1.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git commit -m"commit"
[ft/footer 4f51007] commit
 1 file changed, 12 insertions(+)
 create mode 100644 footer1.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

Eric-2:Gym_Git_Exercise_Solutions mac$  git status
On branch ft/footer
All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)
Eric-2:Gym_Git_Exercise_Solutions mac$ git push --set-upstream origin ft/footer
Counting objects: 8, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 974 bytes | 974.00 KiB/s, done.
Total 8 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), completed with 1 local object.
To https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git
   95fbe27..25ec727  ft/footer -> ft/footer
Branch 'ft/footer' set up to track remote branch 'ft/footer' from 'origin'.
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 8 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)
Eric-2:Gym_Git_Exercise_Solutions mac$  git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
Eric-2:Gym_Git_Exercise_Solutions mac$ git merge --squash ft/footer
Updating 3545ea8..25ec727
Fast-forward
Squash commit -- not updating HEAD
 footer.html  | 12 ++++++++++++
 footer1.html | 12 ++++++++++++
 2 files changed, 24 insertions(+)
 create mode 100644 footer.html
 create mode 100644 footer1.html
Eric-2:Gym_Git_Exercise_Solutions mac$  git add .
Eric-2:Gym_Git_Exercise_Solutions mac$  git commit -m" commting two file"
[ft/squashing 1c5fe3c]  commting two file
 2 files changed, 24 insertions(+)
 create mode 100644 footer.html
 create mode 100644 footer1.html
Eric-2:Gym_Git_Exercise_Solutions mac$ git rebase -i HEAD~2
Successfully rebased and updated refs/heads/ft/squashing.
Eric-2:Gym_Git_Exercise_Solutions mac$ git checkout ft/footer
Switched to branch 'ft/footer'
Your branch is up to date with 'origin/ft/footer'.
Eric-2:Gym_Git_Exercise_Solutions mac$ git merge --squash origin/ft/footer
 (nothing to squash)Already up to date.
Eric-2:Gym_Git_Exercise_Solutions mac$ git status
On branch ft/footer
Your branch is up to date with 'origin/ft/footer'.

nothing to commit, working tree clean
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
fatal: unable to access 'https://github.com/SEBAKUNDA/Gym_Git_Exercise_Solutions.git/': LibreSSL SSL_connect: SSL_ERROR_SYSCALL in connection to github.com:443 
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
Everything up-to-date
Eric-2:Gym_Git_Exercise_Solutions mac$ git push
Everything up-to-date
Eric-2:Gym_Git_Exercise_Solutions mac$ 
```
# bundle 5
# exercise 2
``` bash
Eric-2:git-cafe-exercise mac$  git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")
Eric-2:git-cafe-exercise mac$  git add .
Eric-2:git-cafe-exercise mac$  git commit -m"forked project first commit"
[main bf2bf55] forked project first commit
 1 file changed, 5 insertions(+), 14 deletions(-)
Eric-2:git-cafe-exercise mac$  git push
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 396 bytes | 396.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/SEBAKUNDA/git-cafe-exercise.git
   d1d3f9c..bf2bf55  main -> main
Eric-2:git-cafe-exercise mac$ 
```
