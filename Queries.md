//FOR VERSION OF JAVA 8----------

D:\basics>java -version
java version "1.8.0_202"
Java(TM) SE Runtime Environment (build 1.8.0_202-b08)
Java HotSpot(TM) 64-Bit Server VM (build 25.202-b08, mixed mode)
-------------------------------------------------------------------------
D:\basics>echo %path%
C:\Program Files (x86)\Common Files\Oracle\Java\javapath;C:\oraclexe\app\oracle\product\11.2.0\server\bin;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\System32\OpenSSH\;C:\Program Files\Git\cmd;C:\Program Files\Java\jdk1.8.0_202\bin
----------------------------------------------------------------------------
D:\basics>javac HelloWorld.java

D:\basics>java HelloWorld
HelloWorld
==============================================================================
//FOR VERSION OF JAVA 11
Microsoft Windows [Version 10.0.22621.1555]
(c) Microsoft Corporation. All rights reserved.

D:\basics>java -version
java version "11.0.18" 2023-01-17 LTS
Java(TM) SE Runtime Environment 18.9 (build 11.0.18+9-LTS-195)
Java HotSpot(TM) 64-Bit Server VM 18.9 (build 11.0.18+9-LTS-195, mixed mode)
------------------------------------------------------------------------------
D:\basics>echo %path%
C:\Program Files\Common Files\Oracle\Java\javapath;C:\Program Files (x86)\Common Files\Oracle\Java\javapath;C:\oraclexe\app\oracle\product\11.2.0\server\bin;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\System32\OpenSSH\;C:\Program Files\Git\cmd;C:\Program Files\Java\jdk-11\bin

D:\basics>java HelloWorld
HelloWorld

D:\basics>
-----------------------------------------------------------------------
Q 14. clonning buddie's .class file from git.

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

============================================================================
QUESTION no.15 OUTPUT
D:\basics>javac hello.java
hello.java:1: error: class HelloWorld is public, should be declared in a file named HelloWorld.java
public class HelloWorld
       ^
1 error
=============================================================================
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
===========================================================================
Question no 17 OUTPUT

All done
============================================================================
Question no 18 OUTPUT
After removing path 
java and javac both work.
----------------------------------------------------------------------------
with java output is

Usage: java [options] <mainclass> [args...]
           (to execute a class)
   or  java [options] -jar <jarfile> [args...]
           (to execute a jar file)
   or  java [options] -m <module>[/<mainclass>] [args...]
       java [options] --module <module>[/<mainclass>] [args...]
           (to execute the main class in a module)
   or  java [options] <sourcefile> [args]
           (to execute a single source-file program)

 Arguments following the main class, source file, -jar <jarfile>,
 -m or --module <module>/<mainclass> are passed as the arguments to
 main class.

 where options include:

    -cp <class search path of directories and zip/jar files>
    -classpath <class search path of directories and zip/jar files>
    --class-path <class search path of directories and zip/jar files>
                  A ; separated list of directories, JAR archives,
                  and ZIP archives to search for class files.
    -p <module path>
    --module-path <module path>...
                  A ; separated list of directories, each directory
                  is a directory of modules.
    --upgrade-module-path <module path>...
                  A ; separated list of directories, each directory
                  is a directory of modules that replace upgradeable
                  modules in the runtime image
    --add-modules <module name>[,<module name>...]
                  root modules to resolve in addition to the initial module.
                  <module name> can also be ALL-DEFAULT, ALL-SYSTEM,
                  ALL-MODULE-PATH.
    --list-modules
                  list observable modules and exit
    -d <module name>
    --describe-module <module name>
                  describe a module and exit
    --dry-run     create VM and load main class but do not execute main method.
                  The --dry-run option may be useful for validating the
                  command-line options such as the module system configuration.
    --validate-modules
                  validate all modules and exit
                  The --validate-modules option may be useful for finding
                  conflicts and other errors with modules on the module path.
    -D<name>=<value>
                  set a system property
    -verbose:[class|module|gc|jni]
                  enable verbose output
    -version      print product version to the error stream and exit
    --version     print product version to the output stream and exit
    -showversion  print product version to the error stream and continue
    --show-version
                  print product version to the output stream and continue
    --show-module-resolution
                  show module resolution output during startup
    -? -h -help
                  print this help message to the error stream
    --help        print this help message to the output stream
    -X            print help on extra options to the error stream
    --help-extra  print help on extra options to the output stream
    -ea[:<packagename>...|:<classname>]
    -enableassertions[:<packagename>...|:<classname>]
                  enable assertions with specified granularity
    -da[:<packagename>...|:<classname>]
    -disableassertions[:<packagename>...|:<classname>]
                  disable assertions with specified granularity
    -esa | -enablesystemassertions
                  enable system assertions
    -dsa | -disablesystemassertions
                  disable system assertions
    -agentlib:<libname>[=<options>]
                  load native agent library <libname>, e.g. -agentlib:jdwp
                  see also -agentlib:jdwp=help
    -agentpath:<pathname>[=<options>]
                  load native agent library by full pathname
    -javaagent:<jarpath>[=<options>]
                  load Java programming language agent, see java.lang.instrument
    -splash:<imagepath>
                  show splash screen with specified image
                  HiDPI scaled images are automatically supported and used
                  if available. The unscaled image filename, e.g. image.ext,
                  should always be passed as the argument to the -splash option.
                  The most appropriate scaled image provided will be picked up
                  automatically.
                  See the SplashScreen API documentation for more information
    @argument files
                  one or more argument files containing options
    -disable-@files
                  prevent further argument file expansion
    --enable-preview
                  allow classes to depend on preview features of this release
To specify an argument for a long option, you can use --<name>=<value> or
--<name> <value>.

------------------------------------------------------------------------
output with java is 

C:\Users\Owner>javac
Usage: javac <options> <source files>
where possible options include:
  @<filename>                  Read options and filenames from file
  -Akey[=value]                Options to pass to annotation processors
  --add-modules <module>(,<module>)*
        Root modules to resolve in addition to the initial modules, or all modules
        on the module path if <module> is ALL-MODULE-PATH.
  --boot-class-path <path>, -bootclasspath <path>
        Override location of bootstrap class files
  --class-path <path>, -classpath <path>, -cp <path>
        Specify where to find user class files and annotation processors
  -d <directory>               Specify where to place generated class files
  -deprecation
        Output source locations where deprecated APIs are used
  --enable-preview
        Enable preview language features. To be used in conjunction with either -source or --release.
  -encoding <encoding>         Specify character encoding used by source files
  -endorseddirs <dirs>         Override location of endorsed standards path
  -extdirs <dirs>              Override location of installed extensions
  -g                           Generate all debugging info
  -g:{lines,vars,source}       Generate only some debugging info
  -g:none                      Generate no debugging info
  -h <directory>
        Specify where to place generated native header files
  --help, -help, -?            Print this help message
  --help-extra, -X             Print help on extra options
  -implicit:{none,class}
        Specify whether or not to generate class files for implicitly referenced files
  -J<flag>                     Pass <flag> directly to the runtime system
  --limit-modules <module>(,<module>)*
        Limit the universe of observable modules
  --module <module-name>, -m <module-name>
        Compile only the specified module, check timestamps
  --module-path <path>, -p <path>
        Specify where to find application modules
  --module-source-path <module-source-path>
        Specify where to find input source files for multiple modules
  --module-version <version>
        Specify version of modules that are being compiled
  -nowarn                      Generate no warnings
  -parameters
        Generate metadata for reflection on method parameters
  -proc:{none,only}
        Control whether annotation processing and/or compilation is done.
  -processor <class1>[,<class2>,<class3>...]
        Names of the annotation processors to run; bypasses default discovery process
  --processor-module-path <path>
        Specify a module path where to find annotation processors
  --processor-path <path>, -processorpath <path>
        Specify where to find annotation processors
  -profile <profile>
        Check that API used is available in the specified profile
  --release <release>
        Compile for a specific VM version. Supported targets: 6, 7, 8, 9, 10, 11
  -s <directory>               Specify where to place generated source files
  -source <release>
        Provide source compatibility with specified release
  --source-path <path>, -sourcepath <path>
        Specify where to find input source files
  --system <jdk>|none          Override location of system modules
  -target <release>            Generate class files for specific VM version
  --upgrade-module-path <path>
        Override location of upgradeable modules
  -verbose                     Output messages about what the compiler is doing
  --version, -version          Version information
  -Werror                      Terminate compilation if warnings occur

-------------------------------------------------------------------------------
output with java -version is

C:\Users\Owner>java -version
java version "11.0.18" 2023-01-17 LTS
Java(TM) SE Runtime Environment 18.9 (build 11.0.18+9-LTS-195)
Java HotSpot(TM) 64-Bit Server VM 18.9 (build 11.0.18+9-LTS-195, mixed mode)
==============================================================================

Q 19 .........................................................................
Source file is....
class Main
{
    public static void main(String[] args) {
        String name="bhupendra verma";
        System.out.println(name);
    }
}
----------------------------------------------------------------------------
.class file totaly different from the source file. .class file is

Êþº¾   7 
   	  
       <init> ()V Code LineNumberTable main ([Ljava/lang/String;)V 
SourceFile 	Main.java    bhupendra verma         Main java/lang/Object java/lang/System out Ljava/io/PrintStream; java/io/PrintStream  println (Ljava/lang/String;)V                	        *· ±    
        	 
   	   +     
L² +¶ ±    
          
   
    

============================================================================
Q 20.

Variable name start with number is giving error
==========================================================================
Q 21. 
source code with reseve word as a variable.............................
public class Q21 {
    public static void main(String[] args) {
        String true="bhupendra verma in keyword";
        System.out.println(true);
    }
}
output...............................
PS D:\basics> javac Q21.java
Q21.java:3: error: not a statement
        String true="bhupendra verma in keyword";
        ^
Q21.java:3: error: ';' expected
        String true="bhupendra verma in keyword";
              ^
2 errors

source code with class as variables..................................
public class Q21 {
    public static void main(String[] args) {
        String String="bhupendra verma in String";
        System.out.println(String);
    }
}
output.......................................
PS D:\basics> javac Q21.java
PS D:\basics> java Q21      
bhupendra verma in String
PS D:\basics> 

====================================================================
Q 22...
Nested comment does not work because when we close inner comment first it close the outer comment because inner comment getting comment and does not known by compiler thus outer closing comment has no opening comment because and code give error
=======================================================================
Q 23.
public class Q23 {
    public static void main(String[] args) {
        //printing a string 'Bhupendra Verma'.
        System.out.println("Bhupendra Verma");
    }
}
Output....................
PS D:\basics> javac Q23.java
PS D:\basics> java Q23
Bhupendra Verma
PS D:\basics> 
===========================================================================
