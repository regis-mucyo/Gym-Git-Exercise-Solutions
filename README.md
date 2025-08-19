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

# Bundle 2

## Exercise 1

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add .
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'setup new file'
[ft/bundle-2 cde043c] setup new file
 1 file changed, 10 insertions(+)
 create mode 100644 services.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 434 bytes | 217.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
```

## Exercise 2

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git pull origin main
remote: Enumerating objects: 2, done.
remote: Counting objects: 100% (2/2), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (2/2), 1.78 KiB | 455.00 KiB/s, done.
From https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
   13da3f8..6b5d0e0  main       -> origin/main
Updating 13da3f8..6b5d0e0
Fast-forward
 README.md     | 130 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 about.html    |  10 +++++
 home.html     |  10 +++++
 services.html |  10 +++++
 4 files changed, 160 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add .
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'redesign service page'
[ft/service-redesign fa8d529] redesign service page
 1 file changed, 1 insertion(+)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 368 bytes | 368.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add services.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'Redesign service page for responsive'
[main be9de37] Redesign service page for responsive
 1 file changed, 1 insertion(+)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 336 bytes | 336.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
   6b5d0e0..be9de37  main -> main
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git diff
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git diff ft/service-redesign main
diff --git a/services.html b/services.html
index 3b1d461..d18e9b0 100644
--- a/services.html
+++ b/services.html
@@ -6,6 +6,6 @@
   </head>
   <body>
     <p>This is services page!</p>
-    <p>We Provide Different Services That Can Help You In Self-Development</p>
+    <p>Our Services are Valuable</p>
   </body>
 </html>
(END)
+++ b/services.html
@@ -6,6 +6,6 @@
   </head>
   <body>
     <p>This is services page!</p>
-    <p>We Provide Different Services That Can Help You In Self-Development</p>
+    <p>Our Services are Valuable</p>
   </body>
 </html>
(END)
+++ b/services.html
@@ -6,6 +6,6 @@
   </head>
   <body>
     <p>This is services page!</p>
-    <p>We Provide Different Services That Can Help You In Self-Development</p>
+    <p>Our Services are Valuable</p>
   </body>
 </html>
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch --show-current
ft/service-redesign
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git merge ft/service redesign
merge: ft/service - not something we can merge
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git merge ft/service-redesign
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add services.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'solve conflict between main branch and ft/service-redesign'
[main f704399] solve conflict between main branch and ft/service-redesign
 1 file changed, 1 deletion(-)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 319 bytes | 319.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
   7cb91d5..f704399  main -> main
```
