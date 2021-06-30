# Introduction

 ### what is git? 

1. It's a verion control sysytem
2. It's let you make changes wheere ever you are. This can you can code out side of you hard wear computer.
3. A history of what you have done is save onto your git
4. The ability to, view, apple,and chnage.
5. keep everything in order file.

### Without version conionl

 **co
 mmits** mean to save the work that you have done.
   - you can always go back and fix the work that you have done on on the topic.

### what are my output for the ***terminal*** 
> You have...
    1.git status >what you do know what's going on 
    2.git push  > 
    3.git pull 
    3. ls 
    4. cd 
    5. git commit m- "something"
    6. git add 
if you need more information about them you can go to [git](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)
### Example

projects$ git status 
fatal: not a git repository (or any of the parent directories): .git
projects$ ls 
Reading-notes   courses
projects$ cd Reading-notes
Reading-notes[main *]$ ls 
README.md       _config.yml     git.md          markdown.md
Reading-notes[main *]$ cd git.md
bash: cd: git.md: Not a directory
Reading-notes[main *]$ ls 
README.md       _config.yml     git.md          markdown.md
Reading-notes[main *]$ git status 
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
Reading-notes[main *]$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/JerrodBolton/Reading-notes.git
   d4d7bbd..89e742e  main -> main
Reading-notes[main]$ git status                                  On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
Reading-notes[main]$ git status 
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   git.md

no changes added to commit (use "git add" and/or "git commit -a")
Reading-notes[main !]$ git add .
Reading-notes[main !]$ git commit -m "text"
[main c4d244b] text
 Committer: JerrodBolton <rodrod1@JerrodBltonsMBP.hsd1.tn.comcast.net>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+), 6 deletions(-)
Reading-notes[main *]$ git status 
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
Reading-notes[main *]$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 279 bytes | 279.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/JerrodBolton/Reading-notes.git
   89e742e..c4d244b  main -> main
Reading-notes[main]$ git status 
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
Reading-notes[main]$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
Reading-notes[main]$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 655 bytes | 131.00 KiB/s, done.
From https://github.com/JerrodBolton/Reading-notes
   c4d244b..d2c2222  main       -> origin/main
Updating c4d244b..d2c2222
Fast-forward
 git.md | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)
Reading-notes[main]$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean