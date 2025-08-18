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
