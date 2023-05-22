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

##Exercise 2

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
