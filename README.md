# Bundle 1
## Exercise 1

```
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> echo "# Gym-Git-E>> git init
>> git add README.md
>> git remote add origin https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git
>> git push -u origin main
Initialized empty Git repository in C:/Users/Hp/Desktop/Gym-Git-Exercise-Solutions/.git/
[master (root-commit) 46956f5] first commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Branch 'main' set up to track remote branch 'main' from 'origin'.   
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch main
Your branch is behind 'origin/main' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

nothing to commit, working tree clean
ev
On branch dev
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git push origin dev
remote: Create a pull request for 'dev' on GitHub by visiting:      
remote:      https://github.com/nili-alu/Gym-Git-Exercise-Solutions/remote:
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git       
 * [new branch]      dev -> dev
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch dev
nothing to commit, working tree clean
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:     
remote:      https://github.com/nili-alu/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git       
 * [new branch]      test -> test
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git checkout dev 
Switched to branch 'dev'
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git branch -d test
Deleted branch test (was 46956f5).
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch dev
nothing to commit, working tree clean
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git branch --delete test
error: branch 'test' not found.
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git push origin --delete test
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git
 - [deleted]         test
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> 

```

# Bundle 1
## Exercise 2

```
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git add home.html

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch dev
Changes to be committed:
        new file:   home.html

Saved working directory and index state WIP on dev: 46956f5 first commit
On branch dev
nothing to commit, working tree clean
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash list   
stash@{0}: WIP on dev: 46956f5 first commit
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git staus        
git: 'staus' is not a git command. See 'git --help'.

On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)    
        about.html

o track)
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git add about.htmPS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash        
Saved working directory and index state WIP on dev: 46956f5 first commit
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash list   
stash@{0}: WIP on dev: 46956f5 first commit
stash@{1}: WIP on dev: 46956f5 first commit
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)    
        team.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git add team.html

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash        
mmit
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash list   
stash@{0}: WIP on dev: 46956f5 first commit
stash@{1}: WIP on dev: 46956f5 first commit
stash@{2}: WIP on dev: 46956f5 first commit
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash pop stash@{1}
usage: git stash pop [--index] [-q|--quiet] [<stash>]
    --index               attempt to recreate the index

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash pop stash@{2}
error: unknown switch `e'
usage: git stash pop [--index] [-q|--quiet] [<stash>]
    --index               attempt to recreate the index

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash pop 1  
On branch dev
        new file:   about.html

Dropped refs/stash@{1} (8152a043cbefa3ff96f6f4ba0d3bcfb3872e2853)   
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash list   
stash@{0}: WIP on dev: 46956f5 first commit
stash@{1}: WIP on dev: 46956f5 first commit
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash pop 1  
On branch dev
Changes to be committed:
        new file:   about.html
        new file:   home.html
Dropped refs/stash@{1} (118063b235336b92630e1173b422a46ce836b2d9)   
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git add -all     
error: did you mean `--all` (with two dashes)?
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git add --all    
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch dev
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git commit -m "home an about pages added"
[dev 5659b75] home an about pages added
 2 files changed, 27 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 567 bytes | 94.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git       
   46956f5..5659b75  dev -> dev
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch dev
nothing to commit, working tree clean
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git stash pop    
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (0161bd592598f842f94ed62e971399068f1563b1)   
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git reset --hard 
HEAD is now at 5659b75 home an about pages added
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch dev
nothing to commit, working tree clean
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> 

```

# Bundle 2 
## Exercise 2

``` 

Switched to branch 'main'
rwarded.
  (use "git pull" to update your local branch)
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git pull
Updating 46956f5..6830d69
Fast-forward
 README.md     | Bin 62 -> 7534 bytes
 about.html    |  14 ++++++++++++++
 services.html |  14 ++++++++++++++
 4 files changed, 41 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git status       
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)        
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")   
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git add services.ndle 2, exercise 2"
[ft/service-redesign c53b3eb] bundle 2, exercise 2
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use      

    git push --set-upstream origin ft/service-redesign

PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 343 bytes | 68.00 KiB/s, done.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub byremote:      https://github.com/nili-alu/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git       
 * [new branch]      ft/service-redesign -> ft/service-redesign     
Branch 'ft/service-redesign' set up to track remote branch 'ft/service-redesign' from 'origin'.
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git checkout main

Switched to branch 'main'
Your branch is up to date with 'origin/main'.
On branch main
Your branch is up to date with 'origin/main'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)        
  (use "git restore <file>..." to discard changes in working directomit -m "learn how to solve conflict"
[main ff57cc7] learn how to solve conflict


[ft/service-redesign 48ebe75] Merge branch 'main' into ft/service-redesign                                          result.
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git merge
Already up to date.
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 376 bytes | 125.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0      
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git
   c53b3eb..48ebe75  ft/service-redesign -> ft/service-redesign
PS C:\Users\Hp\Desktop\Gym-Git-Exercise-Solutions> 
```

# Bundle 3 
## Exercise 1

``` 

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.


nothing to commit, working tree clean

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/team-page)
$ git add team.html

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/team-page)
$ git commit -m "team page added"
[ft/team-page 93be0b3] team page added
 1 file changed, 12 insertions(+)     
 create mode 100644 team.html

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page


Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 464 bytes | 232.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/nili-alu/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
Branch 'ft/team-page' set up to track remote branch 'ft/team-page' from 'origin'.

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 1 commit, and can be 
fast-forwarded.
  (use "git pull" to update your local branch)

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.       

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/team-page)
$ git log
commit 93be0b3ec6338aecffb31f1ca217e51c9e3e1dcb (HEAD -> ft/team-page, origin/ft/team-page)
Author: Lievin <l.niyoyandi@alustudent.com>
Date:   Mon May 22 18:42:09 2023 +0300

    team page added

commit 48ebe75634c484057a9aa4378a48c4a403e3397e (origin/ft/service-redesign, ft/service-redesign)
Merge: c53b3eb ff57cc7
Author: Lievin <l.niyoyandi@alustudent.com>
Date:   Mon May 22 13:41:32 2023 +0300

    Merge branch 'main' into ft/service-redesign

commit ff57cc71de3fd8ea3feb6d89d8d51d9bf9ad5959 (main, ft/contact-page)
Author: Lievin <l.niyoyandi@alustudent.com>
Date:   Mon May 22 13:29:32 2023 +0300

    learn how to solve conflict

commit c53b3eb7901c39a3c463345ddfa85e0a52cfc029
Author: Lievin <l.niyoyandi@alustudent.com>
Date:   Mon May 22 13:21:22 2023 +0300

    bundle 2, exercise 2

commit 6830d698909109a960963cf5f29e84d2afec75dc
Merge: 1e7287a 00fd8fb
Author: ALVINdimpos <49131269+ALVINdimpos@users.noreply.github.com>

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/team-page)
$

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
b git cherry-pick 93be0b3ec6338aecffb31f1ca217e51c9e3e1dcb
[ft/contact-page 8dac584] team page added
 Date: Mon May 22 18:42:09 2023 +0300
 1 file changed, 12 insertions(+)
 create mode 100644 team.html

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html

nothing added to commit but untracked files present (use "git add" to track)

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git add contact.html

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git commit -m 'contact page"
> ^C

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git commit -m "contact page created"
[ft/contact-page 5a026ad] contact page created
 1 file changed, 12 insertions(+)
 create mode 100644 contact.html

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page


Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 731 bytes | 731.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/nili-alu/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page     
Branch 'ft/contact-page' set up to track remote branch 'ft/contact-page' from 'origin'.

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout -b ft/fag-page
Switched to a new branch 'ft/fag-page'

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$ git status
On branch ft/fag-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        fag.html

nothing added to commit but untracked files present (use "git add" to track)

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$ git add fag.html

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$ git commit -m "fag page created"
[ft/fag-page a17532f] fag page created
 1 file changed, 12 insertions(+)
 create mode 100644 fag.html

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$ git push
fatal: The current branch ft/fag-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/fag-page


Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$ git push --set-upstream origin ft/fag-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 467 bytes | 233.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/fag-page' on GitHub by visiting:
remote:      https://github.com/nili-alu/Gym-Git-Exercise-Solutions/pull/new/ft/fag-page
remote:
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/fag-page -> ft/fag-page
Branch 'ft/fag-page' set up to track remote branch 'ft/fag-page' from 'origin'.

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$ git log
commit a17532faf0a84fe6f0811018966dd9805d3819fa (HEAD -> ft/fag-page, origin/ft/fag-page)
Author: Lievin <l.niyoyandi@alustudent.com>
Date:   Mon May 22 19:02:56 2023 +0300

Revert "team page added"
    fag page created

commit 5a026ad8f30d3719fea8da736e6ce9321455dee4 (origin/ft/contact-page, ft/contact-page)
Author: Lievin <l.niyoyandi@alustudent.com>
Date:   Mon May 22 18:58:07 2023 +0300

    contact page created

commit 8dac584e9ee3d23d412f58c608f4ef9cf98d7536
Author: Lievin <l.niyoyandi@alustudent.com>
Date:   Mon May 22 18:42:09 2023 +0300

    team page added

commit ff57cc71de3fd8ea3feb6d89d8d51d9bf9ad5959 (main)      
Author: Lievin <l.niyoyandi@alustudent.com>
Date:   Mon May 22 13:29:32 2023 +0300

    learn how to solve conflict

commit 6830d698909109a960963cf5f29e84d2afec75dc
Merge: 1e7287a 00fd8fb
Author: ALVINdimpos <49131269+ALVINdimpos@users.noreply.github.com>
Date:   Mon May 22 12:15:53 2023 +0200


Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$ git revert 8dac584e9ee3d23d412f58c608f4ef9cf98d7536       
Removing team.html
[ft/fag-page d0abe2e] Revert "team page added"
                                               1 file changed, 12 deletions(-)
                   delete mode 100644 team.html

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 275 bytes | 275.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/nili-alu/Gym-Git-Exercise-Solutions.git
   a17532f..d0abe2e  ft/fag-page -> ft/fag-page

Hp@LIEVIN-1999NIYO MINGW64 ~/Desktop/Gym-Git-Exercise-Solutions (ft/fag-page)
$
```
