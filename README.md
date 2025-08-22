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

# Bundle 3

## Exercise 1

```bash
PS D:\The Gym's\PHASE 2\Git Learning> cd '.\Git Exercises\'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add team.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'setup team file and add contents'
[ft/team-page 779dccc] setup team file and add contents
 1 file changed, 13 insertions(+)
 create mode 100644 team.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 486 bytes | 486.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises>
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout ft/team-page
Switched to branch 'ft/team-page'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git log
commit 779dccc810f04130157feb0f93ef09ee0e5fcb0e (HEAD -> ft/team-page, origin/ft/team-page)
Author: Regis Mucyo <mucyoregis250@gmail.com>
Date:   Wed Aug 20 14:12:30 2025 +0200

    setup team file and add contents

commit 34a7354e775a52b12658fa18f1841edb61e5bb58 (origin/main, main, ft/contact-page)
Author: Regis Mucyo <mucyoregis250@gmail.com>
Date:   Tue Aug 19 17:02:44 2025 +0200

    Exercise 2 from bundle 2
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout ft/contact-page
Switched to branch 'ft/contact-page'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git log ft/team-page --oneline
779dccc (origin/ft/team-page, ft/team-page) setup team file and add contents
34a7354 (HEAD -> ft/contact-page, origin/main, main) Exercise 2 from bundle 2
f704399 solve conflict between main branch and ft/service-redesign
7cb91d5 Merge branch 'ft/service-redesign'
be9de37 Redesign service page for responsive
fa8d529 (origin/ft/service-redesign, ft/service-redesign) redesign service page
6b5d0e0 Merge pull request #4 from regis-mucyo/ft/bundle-2
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> ^C
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch --show-current
ft/contact-page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git cherry-pick 779dccc
[ft/contact-page b84f653] setup team file and add contents
 Date: Wed Aug 20 14:12:30 2025 +0200
 1 file changed, 13 insertions(+)
 create mode 100644 team.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add contact.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'Setup contanct page and add contents'
[ft/contact-page 729aa28] Setup contanct page and add contents
 1 file changed, 10 insertions(+)
 create mode 100644 contact.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 898 bytes | 299.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add faq.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'setup a new page for FAQ'
[ft/faq-page 5f5a419] setup a new page for FAQ
 1 file changed, 10 insertions(+)
 create mode 100644 faq.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 453 bytes | 453.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git log --oneline
5f5a419 (HEAD -> ft/faq-page, origin/ft/faq-page) setup a new page for FAQ
729aa28 (origin/ft/contact-page, ft/contact-page) Setup contanct page and add contents
b84f653 setup team file and add contents
34a7354 (origin/main, main) Exercise 2 from bundle 2
f704399 solve conflict between main branch and ft/service-redesign
7cb91d5 Merge branch 'ft/service-redesign'
be9de37 Redesign service page for responsive
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch --show-current
ft/faq-page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git revert 779dccc
[ft/faq-page 587e064] Revert "fix a bug in team file"
 1 file changed, 13 deletions(-)
 delete mode 100644 team.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git log --oneline
587e064 (HEAD -> ft/faq-page) Revert "fix a bug in team file"
5f5a419 (origin/ft/faq-page) setup a new page for FAQ
729aa28 (origin/ft/contact-page, ft/contact-page) Setup contanct page and add contents
b84f653 setup team file and add contents
34a7354 (origin/main, main) Exercise 2 from bundle 2
f704399 solve conflict between main branch and ft/service-redesign
7cb91d5 Merge branch 'ft/service-redesign'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch --show-current
ft/faq-page
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git status
On branch ft/faq-page
nothing to commit, working tree clean
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 279 bytes | 279.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
   5f5a419..587e064  ft/faq-page -> ft/faq-page
```

## Exercise 2

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
........
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add home.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'update page from home page'
[main a12ca3b] update page from home page
 1 file changed, 1 insertion(+), 1 deletion(-)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/home-page-redesign
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesigning -> ft/home-page-redesign
.........
 *  History restored

PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git branch --show-current
ft/home-page-redesign
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add home.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'add heading'
[ft/home-page-redesign a499380] add heading
 1 file changed, 2 insertions(+), 1 deletion(-)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/home-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 16 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.79 KiB | 229.00 KiB/s, done.
Total 14 (delta 6), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (6/6), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
```

# Bundle 4

## Exercise 1

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git remote -v
origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git (fetch)
origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git (push)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git remote add git-copy https://github.com/regis-mucyo/git-copy.git
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git remote -v
git-copy        https://github.com/regis-mucyo/git-copy.git (fetch)
git-copy        https://github.com/regis-mucyo/git-copy.git (push)
origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git (fetch)
origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git (push)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git remote remove git-copy
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git remote -v
origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git (fetch)
origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git (push)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git remote add git-copy https://github.com/regis-mucyo/git-learning.git
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git remote -v
git-copy        https://github.com/regis-mucyo/git-learning.git (fetch)
git-copy        https://github.com/regis-mucyo/git-learning.git (push)
origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git (fetch)
origin  https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git (push)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add home.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'add new content in homepage'
[main 736fc96] add new content in homepage
 1 file changed, 1 insertion(+)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 364 bytes | 364.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
   44e0186..736fc96  main -> main
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push git-copy
Enumerating objects: 49, done.
Counting objects: 100% (49/49), done.
Delta compression using up to 16 threads
Compressing objects: 100% (46/46), done.
Writing objects: 100% (49/49), 9.79 KiB | 385.00 KiB/s, done.
Total 49 (delta 19), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (19/19), done.
To https://github.com/regis-mucyo/git-learning.git
 * [new branch]      main -> main
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises>
```

## Exercise 2

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b ft/footer
Switched to a new branch 'ft/footer'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add services.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'Add services list'
[ft/footer 9ef9389] Add services list
 1 file changed, 7 insertions(+)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git add --all
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'insert new contents'
[ft/footer b545e85] insert new contents
 3 files changed, 7 insertions(+)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/footer
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 16 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 979 bytes | 489.00 KiB/s, done.
Total 8 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git log --oneline
78ee170 (HEAD -> ft/squashing, origin/main, main) add history of bundle 4 exercise 1
736fc96 (git-copy/main) add new content in homepage
44e0186 Revert "fix typo error"
5033cb1 Bundle 3 exercise 2 git command history
a12ca3b update page from home page
6aeb530 (origin/ft/home-page-redesigning) update head for home page
4799c3c Add command history of git for Exercise 2 in Bundle 3
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git log --oneline
78ee170 (HEAD -> main, origin/main, ft/squashing) add history of bundle 4 exercise 1
736fc96 (git-copy/main) add new content in homepage
44e0186 Revert "fix typo error"
5033cb1 Bundle 3 exercise 2 git command history
a12ca3b update page from home page
6aeb530 (origin/ft/home-page-redesigning) update head for home page
4799c3c Add command history of git for Exercise 2 in Bundle 3
34a7354 Exercise 2 from bundle 2
f704399 solve conflict between main branch and ft/service-redesign
7cb91d5 Merge branch 'ft/service-redesign'
be9de37 Redesign service page for responsive
fa8d529 (origin/ft/service-redesign, ft/service-redesign) redesign service page
6b5d0e0 Merge pull request #4 from regis-mucyo/ft/bundle-2
6f3fc0e (origin/ft/bundle-2, ft/bundle-2) Add Git Commands history for exercise 1 in bundle 2
d4d48b1 Merge pull request #3 from regis-mucyo/ft/bundle-2
cde043c setup new file
46eb17d (origin/dev, dev) Second exercise in bundle 1
3bf43f5 setup home and about files
50388e6 first exercise in bundle one
13da3f8 initial first commit
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout ft/footer
Switched to branch 'ft/footer'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git log --oneline
b545e85 (HEAD -> ft/footer, origin/ft/footer) insert new contents
9ef9389 Add services list
78ee170 (origin/main, main, ft/squashing) add history of bundle 4 exercise 1
736fc96 (git-copy/main) add new content in homepage
44e0186 Revert "fix typo error"
5033cb1 Bundle 3 exercise 2 git command history
a12ca3b update page from home page
6aeb530 (origin/ft/home-page-redesigning) update head for home page
4799c3c Add command history of git for Exercise 2 in Bundle 3
34a7354 Exercise 2 from bundle 2
f704399 solve conflict between main branch and ft/service-redesign
7cb91d5 Merge branch 'ft/service-redesign'
be9de37 Redesign service page for responsive
fa8d529 (origin/ft/service-redesign, ft/service-redesign) redesign service page
6b5d0e0 Merge pull request #4 from regis-mucyo/ft/bundle-2
6f3fc0e (origin/ft/bundle-2, ft/bundle-2) Add Git Commands history for exercise 1 in bundle 2
d4d48b1 Merge pull request #3 from regis-mucyo/ft/bundle-2
cde043c setup new file
46eb17d (origin/dev, dev) Second exercise in bundle 1
3bf43f5 setup home and about files
50388e6 first exercise in bundle one
13da3f8 initial first commit
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git checkout ft/squashing
Switched to branch 'ft/squashing'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git merge --squash
fatal: No remote for the current branch.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git merge --squash ft/footer
Updating 78ee170..b545e85
Fast-forward
Squash commit -- not updating HEAD
 about.html    |  1 +
 home.html     |  1 +
 services.html | 12 ++++++++++++
 3 files changed, 14 insertions(+)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git log --oneline
78ee170 (HEAD -> ft/squashing, origin/main, main) add history of bundle 4 exercise 1
736fc96 (git-copy/main) add new content in homepage
44e0186 Revert "fix typo error"
5033cb1 Bundle 3 exercise 2 git command history
a12ca3b update page from home page
6aeb530 (origin/ft/home-page-redesigning) update head for home page
4799c3c Add command history of git for Exercise 2 in Bundle 3
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git status
On branch ft/squashing
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   about.html
        modified:   home.html
        modified:   services.html

PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git commit -m 'footer changes squashing'
[ft/squashing 8961b58] footer changes squashing
 3 files changed, 14 insertions(+)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises> git push origin ft/squashing
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 16 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 740 bytes | 246.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote:
To https://github.com/regis-mucyo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
```

# Bundle 5

## Exercise 2

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned> cd .\git-cafe-exercise\
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git add index.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git commit -m 'fix: update the home page head'
[main 38fdace] fix: update the home page head
 1 file changed, 399 insertions(+), 239 deletions(-)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.56 KiB | 800.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/regis-mucyo/git-cafe-exercise.git
   d1d3f9c..38fdace  main -> main
```

# Bundle 6

## Exercise 1

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git checkout -b feat/update-menu
Switched to a new branch 'feat/update-menu'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git status
On branch feat/update-menu
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   css/style.css
        modified:   index-3.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git add --all
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git commit -m 'update image borders'
[feat/update-menu 222f598] update image borders
 2 files changed, 329 insertions(+), 165 deletions(-)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git push origin feat/update-menu
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 16 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1.51 KiB | 774.00 KiB/s, done.
Total 5 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), completed with 4 local objects.
remote:
remote: Create a pull request for 'feat/update-menu' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/git-cafe-exercise/pull/new/feat/update-menu
remote:
To https://github.com/regis-mucyo/git-cafe-exercise.git
 * [new branch]      feat/update-menu -> feat/update-menu
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise>
```

## Exercise 2

```bash
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git checkout -b bugfix/rename-file
Switched to a new branch 'bugfix/rename-file'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git branch -d bugfix/rename-file
error: the branch 'bugfix/rename-file' is not fully merged
hint: If you are sure you want to delete it, run 'git branch -D bugfix/rename-file'
hint: Disable this message with "git config set advice.forceDeleteBranch false"
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git branch -D bugfix/rename-file
Deleted branch bugfix/rename-file (was 222f598).
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git checkout -b bugfix/rename-title
Switched to a new branch 'bugfix/rename-title'
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git status
On branch bugfix/rename-title
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index-4.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git add index-4.html
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git commit -m 'fix bug of title name'
[bugfix/rename-title c30f6c2] fix bug of title name
 1 file changed, 232 insertions(+), 164 deletions(-)
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise> git push origin bugfix/rename-title
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.41 KiB | 724.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'bugfix/rename-title' on GitHub by visiting:
remote:      https://github.com/regis-mucyo/git-cafe-exercise/pull/new/bugfix/rename-title
remote:
To https://github.com/regis-mucyo/git-cafe-exercise.git
 * [new branch]      bugfix/rename-title -> bugfix/rename-title
PS D:\The Gym's\PHASE 2\Git Learning\Git Exercises\cloned\git-cafe-exercise>
```
