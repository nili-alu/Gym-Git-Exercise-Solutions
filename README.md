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
