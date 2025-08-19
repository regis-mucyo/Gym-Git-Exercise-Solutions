# Git Exercises

# Bundle 1

## Exercise 1

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git init
Initialized empty Git repository in D:/The Gym's/PHASE 2/Git Learning/Git Exercises/.git/
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch -M main
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add .
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m "initial first commit"
[main (root-commit) 13da3f8] initial first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git remote add origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 238 bytes | 238.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b dev
Switched to a new branch 'dev'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b test
Switched to a new branch 'test'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch -d test
error: cannot delete branch 'test' used by worktree at 'D:/The Gym's/PHASE 2/Git Learning/Git Exercises'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout dev
Switched to branch 'dev'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch -d test
Deleted branch test (was 13da3f8).
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch --show-current
dev
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
```

## Exercise 2

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add --all
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git stash push -m 'home page'
Saved working directory and index state On dev: home page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add --all
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git stash push -m 'about page'
Saved working directory and index state On dev: about page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add .
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git stash push -m 'team page'
Saved working directory and index state On dev: team page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git stash list
stash@{0}: On dev: team page
stash@{1}: On dev: about page
stash@{2}: On dev: home page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git stash pop 'stash@{2}'
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{2} (1ba3c9a9618ab4b1632fa437efcb56c2c620bce2)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git stash pop 'stash@{1}'
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (b1869aae154681461c6a23cca7ecf1e5966b5720)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add --all
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'setup home and about files'
[dev 3bf43f5] setup home and about files
 2 files changed, 20 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 546 bytes | 273.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
   50388e6..3bf43f5  dev -> dev
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git stash pop 'stash@{0}'
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (05dacc47a5dcebc9fd45de4520aef08cff6c56ce)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git reset --hard
HEAD is now at 3bf43f5 setup home and about files
```
