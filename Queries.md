//FOR VERSION OF JAVA 8----------

D:\basics>java -version
java version "1.8.0_202"
Java(TM) SE Runtime Environment (build 1.8.0_202-b08)
Java HotSpot(TM) 64-Bit Server VM (build 25.202-b08, mixed mode)

D:\basics>echo %path%
C:\Program Files (x86)\Common Files\Oracle\Java\javapath;C:\oraclexe\app\oracle\product\11.2.0\server\bin;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\System32\OpenSSH\;C:\Program Files\Git\cmd;C:\Program Files\Java\jdk1.8.0_202\bin

D:\basics>javac HelloWorld.java

D:\basics>java HelloWorld
HelloWorld

//FOR VERSION OF JAVA 11
Microsoft Windows [Version 10.0.22621.1555]
(c) Microsoft Corporation. All rights reserved.

D:\basics>java -version
java version "11.0.18" 2023-01-17 LTS
Java(TM) SE Runtime Environment 18.9 (build 11.0.18+9-LTS-195)
Java HotSpot(TM) 64-Bit Server VM 18.9 (build 11.0.18+9-LTS-195, mixed mode)

D:\basics>echo %path%
C:\Program Files\Common Files\Oracle\Java\javapath;C:\Program Files (x86)\Common Files\Oracle\Java\javapath;C:\oraclexe\app\oracle\product\11.2.0\server\bin;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\System32\OpenSSH\;C:\Program Files\Git\cmd;C:\Program Files\Java\jdk-11\bin

D:\basics>java HelloWorld
HelloWorld

D:\basics>

//After making private repo

Owner@Bhuvie MINGW64 /d/buddy(pragyan) (master)
$ git clone git@github.com:Pragyanraj23/java.git
fatal: destination path 'java' already exists and is not an empty directory.

//After deleting java repo from git
Owner@Bhuvie MINGW64 /d/buddy(pragyan) (master)
$ git clone https://github.com/Pragyanraj23/java.git
Cloning into 'java'...
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 9 (delta 0), reused 6 (delta 0), pack-reused 0
Receiving objects: 100% (9/9), done.

Owner@Bhuvie MINGW64 /d/buddy(pragyan) (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        java/

nothing added to commit but untracked files present (use "git add" to track)

Owner@Bhuvie MINGW64 /d/buddy(pragyan) (master)
$ cd java

Owner@Bhuvie MINGW64 /d/buddy(pragyan)/java (master)
$ ls
Queries.md  readme.md


Owner@Bhuvie MINGW64 /d/buddy(pragyan)/java (master)
$ notepad readme.md

Owner@Bhuvie MINGW64 /d/buddy(pragyan)/java (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")

Owner@Bhuvie MINGW64 /d/buddy(pragyan)/java (master)
$ git add -A

Owner@Bhuvie MINGW64 /d/buddy(pragyan)/java (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   readme.md


Owner@Bhuvie MINGW64 /d/buddy(pragyan)/java (master)
$ git commit -m "commited after making repo private"
[master bb368e7] commited after making repo private
 1 file changed, 4 insertions(+), 1 deletion(-)

Owner@Bhuvie MINGW64 /d/buddy(pragyan)/java (master)
$ git remote -v
origin  https://github.com/Pragyanraj23/java.git (fetch)
origin  https://github.com/Pragyanraj23/java.git (push)

Owner@Bhuvie MINGW64 /d/buddy(pragyan)/java (master)
$ git push origin master
To https://github.com/Pragyanraj23/java.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/Pragyanraj23/java.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

QUESTION no.15 OUTPUT
D:\basics>javac hello.java
hello.java:1: error: class HelloWorld is public, should be declared in a file named HelloWorld.java
public class HelloWorld
       ^
1 error

Question no 16 OUTPUT
D:\basics>javac multiclass.java

D:\basics>java multiclass
Multiclass

D:\basics>java multiclass1
class 1

D:\basics>java multiclass2
Class 2

D:\basics>java multiclass3
class 3

D:\basics>
