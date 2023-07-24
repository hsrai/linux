## UNIX
The Unix shell has been around longer than most of its users have been alive. It has survived because it’s a powerful tool that allows
users to perform complex and powerful tasks, often with just a few keystrokes or lines of code. It helps users automate repetitive tasks 
and easily combine smaller tasks into larger, more powerful workflows.

Use of the shell is fundamental to a wide range of advanced computing tasks, including high-performance computing. These lessons will introduce you to this powerful tool.



This lesson guides you through the basics of file systems and the shell. If you have stored files on a computer at all and recognize 
the word “file” and either “directory” or “folder” (two common words for the same thing), you’re ready for this lesson.

If you’re already comfortable manipulating files and directories, searching for files with grep and find, and writing simple loops and 
scripts, you probably want to explore the next lesson: shell-extras.
# Download files
   1. Download shell-lesson-data.zip and move the file to your Desktop.
    2.Unzip/extract the file. Let your instructor know if you need help with this step. You should end up with a new folder called shell-lesson-data on your Desktop.


# Install software
If you do not already have the shell software installed, you will need to download and install it.

# Open a new shell
    3.Open a terminal. If you’re not sure how to open a terminal on your operating system, see the instructions below.
    4.In the terminal type cd then press the Return key. This step will make sure you start with your home folder as your working directory.

# Where to type commands: How to open a new shell

The shell is a program that enables us to send commands to the computer and receive output. It is also referred to as the terminal or command line.

Some computers include a default Unix Shell program. The steps below describe some methods for identifying and opening a Unix Shell program if you already have one installed. There are also options for identifying and downloading a Unix Shell program, a Linux/UNIX emulator, or a program to access a Unix Shell on a server.

If none of the options below address your circumstances, try an online search for: Unix shell [your computer model] [your operating system]

# The Shell

The shell is a program where users can type commands. With the shell, it’s possible to invoke complicated programs like climate modeling software or simple commands that create an empty directory with only one line of code. The most popular Unix shell is Bash (the Bourne Again SHell — so-called because it’s derived from a shell written by Stephen Bourne). Bash is the default shell on most modern implementations of Unix and in most packages that provide Unix-like tools for Windows. Note that ‘Git Bash’ is a piece of software that enables Windows users to use a Bash like interface when interacting with Git.

## Note that your prompt might look a little different. In particular, most popular shell environments by default put your user name and the host name before the $. Such a prompt might look like, e.g.:
 nelle@localhost $
# Bash
$ ls
# Output
Desktop    Downloads     Music     Public          snap       Videos
Documents  frappe-bench  Pictures  site1.localRai  Templates

 ## If the shell can’t find a program whose name is the command you typed, it will print an error message such as:
 $ ks
 # Output
ks: command not found



