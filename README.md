Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test
$ git status
fatal: not a git repository (or any of the parent directories): .git

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test
$ git init
Initialized empty Git repository in C:/Users/Pc/Desktop/test/.git/

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ touch file33.txt

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ code .

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file33.txt

nothing added to commit but untracked files present (use "git add" to track)

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git add file33.txt

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file33.txt


Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file33.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file33.txt


Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file33.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file33.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file44.txt


Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git add file44.txt

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file33.txt
        new file:   file44.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file33.txt


Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file33.txt
        new file:   file44.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file33.txt
        modified:   file44.txt


Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git commit -m "file33.txt file44.txt done"
[master (root-commit) 4b89a4d] file33.txt file44.txt done
 2 files changed, 4 insertions(+)
 create mode 100644 file33.txt
 create mode 100644 file44.txt

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git add file55.txt

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file55.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file33.txt
        modified:   file44.txt


Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file55.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file33.txt
        modified:   file44.txt
        modified:   file55.txt


Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file55.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file33.txt
        modified:   file44.txt
        modified:   file55.txt


Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git rm --cached "file55.txt"
error: the following file has staged content different from both the
file and the HEAD:
    file55.txt
(use -f to force removal)

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git log
commit 4b89a4d7285a54b2cbf0c77758a3fa6b0d506d6a (HEAD -> master)
Author: ines <inesjlassi37@gmail.com>
Date:   Wed Aug 14 11:48:30 2024 +0200

    file33.txt file44.txt done

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$ git log
commit 4b89a4d7285a54b2cbf0c77758a3fa6b0d506d6a (HEAD -> master)
Author: ines <inesjlassi37@gmail.com>
Date:   Wed Aug 14 11:48:30 2024 +0200

    file33.txt file44.txt done

Pc@DESKTOP-UVC6UP7 MINGW64 ~/Desktop/test (master)
$
