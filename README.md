 backfill   Download missing objects in a partial clone
   branch     List, create, or delete branches
   commit     Record changes to the repository
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   reset      Reset current HEAD to the specified state
   switch     Switch branches
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects
   push       Update remote refs along with associated objects


'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.
PS C:\Users\User\Downloads\79 demo> git config --global user.name "muthu14"
PS C:\Users\User\Downloads\79 demo> git config --global user.email "muthuvisalakshi.m2023ai-ds@sece.ac.in"
PS C:\Users\User\Downloads\79 demo> git clone "https://github.com/muth14/d1.git"
Cloning into 'd1'...
warning: You appear to have cloned an empty repository.
PS C:\Users\User\Downloads\79 demo> cd d1
PS C:\Users\User\Downloads\79 demo\d1> git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)
PS C:\Users\User\Downloads\79 demo\d1> git add 1.txt
PS C:\Users\User\Downloads\79 demo\d1> git commit -m "1.txt"
[main (root-commit) f91e6a3] 1.txt
 1 file changed, 1 insertion(+)
 create mode 100644 1.txt
PS C:\Users\User\Downloads\79 demo\d1> git push origin main
info: please complete authentication in your browser...
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 233 bytes | 233.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/muth14/d1.git
 * [new branch]      main -> main
PS C:\Users\User\Downloads\79 demo\d1> git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 915 bytes | 228.00 KiB/s, done.
From https://github.com/muth14/d1
   f91e6a3..b7d87a9  main       -> origin/main
Updating f91e6a3..b7d87a9
Fast-forward
 2.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 2.txt
PS C:\Users\User\Downloads\79 demo\d1>


S C:\Users\User\Downloads\79 demo> cd d2
PS C:\Users\User\Downloads\79 demo\d2> git branch -a
* main
  remotes/origin/main
PS C:\Users\User\Downloads\79 demo\d2> git branch b1
PS C:\Users\User\Downloads\79 demo\d2> git branch -a
  b1
* main
  remotes/origin/main
PS C:\Users\User\Downloads\79 demo\d2> git checkout b2
error: pathspec 'b2' did not match any file(s) known to git
PS C:\Users\User\Downloads\79 demo\d2> git checkout b2
error: pathspec 'b2' did not match any file(s) known to git
PS C:\Users\User\Downloads\79 demo\d2> git branch b1
fatal: a branch named 'b1' already exists
PS C:\Users\User\Downloads\79 demo\d2> git add 4.txt
PS C:\Users\User\Downloads\79 demo\d2> git checkout b2
error: pathspec 'b2' did not match any file(s) known to git
PS C:\Users\User\Downloads\79 demo\d2> git branch -a
  b1
* main
  remotes/origin/main
PS C:\Users\User\Downloads\79 demo\d2> git pull 
From https://github.com/muth14/d2
 * [new branch]      b2         -> origin/b2
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main

PS C:\Users\User\Downloads\79 demo\d2> git branch -a
  b1
* main
  remotes/origin/b2
  remotes/origin/main
PS C:\Users\User\Downloads\79 demo\d2> git checkout b2
D       3.txt
A       4.txt
branch 'b2' set up to track 'origin/b2'.
Switched to a new branch 'b2'
PS C:\Users\User\Downloads\79 demo\d2> git diff b1
diff --git a/3.txt b/4.txt
similarity index 100%
rename from 3.txt
rename to 4.txt
PS C:\Users\User\Downloads\79 demo\d2> git diff main
diff --git a/3.txt b/4.txt
similarity index 100%
rename from 3.txt
rename to 4.txt
PS C:\Users\User\Downloads\79 demo\d2> git merge main
Already up to date.
PS C:\Users\User\Downloads\79 demo\d2> git merge 



