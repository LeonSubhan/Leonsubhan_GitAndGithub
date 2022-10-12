1. Create a git repository “YourName_GitAndGithub” to your GitHub account and make it public.
Created a fir repository "Lewonsubhan_GitAndGitHub" and it is public.
Here is the link for it: https://github.com/LeonSubhan/Leonsubhan_GitAndGithub.git

2. Clone this repository to your local machine.
leons@LeonSubhan MINGW64 ~/Documents (master)
$ git clone https://github.com/LeonSubhan/Leonsubhan_GitAndGithub.git
Cloning into 'Leonsubhan_GitAndGithub'...
warning: You appear to have cloned an empty repository.

3. Check which branch you are in now. Is it the “Master” branch?
leons@LeonSubhan MINGW64 ~/Documents (master)
$ git log -oneline
fatal: your current branch 'master' does not have any commits yet

4. Add two text files in this “Master” branch. 1. Git. text 2. GitHub.text
leons@LeonSubhan MINGW64 ~/Documents (master)
$ touch Git.txt
leons@LeonSubhan MINGW64 ~/Documents (master)
$ touch GitHub.txt

5. Write something about git and GitHub (at least 100 words) in the respective .text file.
$ cat Git.txt
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed
and efficiency.

Git is easy to learn and has a tiny footprint with lightning fast performance. It outclasses SCM tools like Subversion, CVS, Perforce, and 
ClearCase with features like cheap local branching, convenient staging areas, and multiple workflows.
leons@LeonSubhan MINGW64 ~/Documents (master)
$ cat GitHub.txt
GitHub, Inc. is an Internet hosting service for software development and version control using Git. It provides the distributed version
control of Git plus access control, bug tracking, software feature requests, task management, continuous integration, and wikis for every
project. Headquartered in California, it has been a subsidiary of Microsoft since 2018.

It is commonly used to host open source software development projects. As of June 2022, GitHub reported having over 83 million developers
and more than 200 million repositories, including at least 28 million public repositories. It is the largest source code host as of November
2021.

6. Add a README.md file. write the uses git commands, usage, and answers which you have finished.
leons@LeonSubhan MINGW64 ~/Documents (master)
$ nano README.md

7. See the changes by the respective git command.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Git.txt
        GitHub.txt
        README.md

nothing added to commit but untracked files present (use "git add" to track)

8. Now Push your Changes to remote. and check the remote changes.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git init
Reinitialized existing Git repository in C:/Users/leons/Documents/Leonsubhan_GitAndGithub/.git/

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git commit -m "Test 2 v 1.0"
On branch main

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Git.txt
        GitHub.txt
        README.md

nothing added to commit but untracked files present (use "git add" to track)

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git add .
warning: in the working copy of 'Git.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'GitHub.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git commit -m "Test 2 v 1.0"
[main (root-commit) e53aab6] Test 2 v 1.0
 3 files changed, 47 insertions(+)
 create mode 100644 Git.txt
 create mode 100644 GitHub.txt
 create mode 100644 README.md

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git branch -M main

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git remote add origin https://github.com/LeonSubhan/Leonsubhan_GitAndGithub.git
error: remote origin already exists.

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1.89 KiB | 1.89 MiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/LeonSubhan/Leonsubhan_GitAndGithub.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

9. Add a “temp” folder in the local directory. and some files(image, video) to that folder.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ mkdir temp
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ cd temp
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub/temp (main)
$ ls
'2022-10-11 20-58-05.mkv'  'Screenshot 2022-10-11 205428.png'

10. Add a “.gitignore” file to your local directory.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ touch .gitignore

11. Declare the “temp” folder in the “.gitignore” file because you don’t want to store these files in the remote repository.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ touch temp >> .gitignore


12 See the local changes by the respective git command.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        temp/

nothing added to commit but untracked files present (use "git add" to track)

13. Now-Again push all the changes to the remote repository.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        temp/

nothing added to commit but untracked files present (use "git add" to track)

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git add .

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   temp/2022-10-11 20-58-05.mkv
        new file:   temp/Screenshot 2022-10-11 205428.png


leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git commit -m "Test 2 v 1.1"
[main a1a6500] Test 2 v 1.1
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 .gitignore
 create mode 100644 temp/2022-10-11 20-58-05.mkv
 create mode 100644 temp/Screenshot 2022-10-11 205428.png

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (main)
$ git push -u origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 324.56 KiB | 19.09 MiB/s, done.


Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/LeonSubhan/Leonsubhan_GitAndGithub.git
   e53aab6..a1a6500  main -> main
branch 'main' set up to track 'origin/main'.

14. Add a feature branch “differences” to your repository. Check how many branches you have now. then set your current branch as the “differences” branch. 

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (differences)
$ git branch differences
fatal: a branch named 'differences' already exists

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (differences)
$ git branch -a
* differences
  main
  remotes/origin/main

15. Update the text files (1. Git. text 2. GitHub.text) by writing the features of git and GitHub.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (differences)
$ nano Git.txt

leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (differences)
$ nano GitHub.txt

16. Adds one more file “difference. text”. write differences between git and GitHub on that file.
leons@LeonSubhan MINGW64 ~/Documents/Leonsubhan_GitAndGithub (differences)
$ nano difference.txt

17. Update the README.md file. write the uses git commands, usage, and answers which you have finished.
updated.
