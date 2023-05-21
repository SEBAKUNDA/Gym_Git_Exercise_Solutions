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

