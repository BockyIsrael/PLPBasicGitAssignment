
Matome@Bokang MINGW64 /
$ cd D:/PLPBasicGitAssignment

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment
$ git init
Initialized empty Git repository in D:/PLPBasicGitAssignment/.git/

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git remote add original https://github.com/BockyIsrael/PLPBasicGitAssignment

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git remove -v
git: 'remove' is not a git command. See 'git --help'.

The most similar command is
        remote

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git remote -v
original        https://github.com/BockyIsrael/PLPBasicGitAssignment (fetch)
original        https://github.com/BockyIsrael/PLPBasicGitAssignment (push)

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git add hello.txt
fatal: pathspec 'hello.txt' did not match any files

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ eccho "Hello, world!" > hello.txt
bash: eccho: command not found

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ echo "Hello, world!" > hello.txt

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git add hello.txt
warning: in the working copy of 'hello.txt', LF will be replaced by CRLF the next time Git touches it

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git config core.autocrlf true

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   hello.txt


Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git rm --cached hello.txt
rm 'hello.txt'

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git add hello.txt
warning: in the working copy of 'hello.txt', LF will be replaced by CRLF the next time Git touches it

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git config core.autocrlf true

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git rm --cached hello.txt
rm 'hello.txt'

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git add hello.txt
warning: in the working copy of 'hello.txt', LF will be replaced by CRLF the next time Git touches it

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ nano .giattributes

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git rm --cached -r
fatal: No pathspec was given. Which files should I remove?

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git add .
warning: in the working copy of '.giattributes', LF will be replaced by CRLF the next time Git touches it

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ echo "*text=auto" > .gitattributes

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git rm --cached -r .
rm '.giattributes'
rm 'hello.txt'

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git add .
warning: in the working copy of '.giattributes', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of '.gitattributes', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'hello.txt', LF will be replaced by CRLF the next time Git touches it

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git config --global core.autocrlf true

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ echo "* text=auto" > .gitattributes

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git add --renormalize .

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git commit -m "Normalize line endings using .gitattributes"
[master (root-commit) 9d1c9d7] Normalize line endings using .gitattributes
 3 files changed, 4 insertions(+)
 create mode 100644 .giattributes
 create mode 100644 .gitattributes
 create mode 100644 hello.txt

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git push origin master
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git remote add origin https://github.com/BockyIsrael/PLPBasicGitAssignment.git

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git remote -v
origin  https://github.com/BockyIsrael/PLPBasicGitAssignment.git (fetch)
origin  https://github.com/BockyIsrael/PLPBasicGitAssignment.git (push)
original        https://github.com/BockyIsrael/PLPBasicGitAssignment (fetch)
original        https://github.com/BockyIsrael/PLPBasicGitAssignment (push)

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git push -u origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (5/5), 365 bytes | 182.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/BockyIsrael/PLPBasicGitAssignment/pull/new/master
remote:
To https://github.com/BockyIsrael/PLPBasicGitAssignment.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git commit -m "Add hello.txt Hello, world!"
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git push -u origion master
fatal: 'origion' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$ git push -u origin master
branch 'master' set up to track 'origin/master'.
Everything up-to-date

Matome@Bokang MINGW64 /d/PLPBasicGitAssignment (master)
$
