## UNIX
The Unix shell has been around longer than most of its users have been alive. It has survived because it’s a powerful tool that allows
users to perform complex and powerful tasks, often with just a few keystrokes or lines of code. It helps users automate repetitive tasks 
and easily combine smaller tasks into larger, more powerful workflows.

Use of the shell is fundamental to a wide range of advanced computing tasks, including high-performance computing. These lessons will introduce you to this powerful tool.



This lesson guides you through the basics of file systems and the shell. If you have stored files on a computer at all and recognize 
the word “file” and either “directory” or "folder" (two common words for the same thing), you’re ready for this lesson.

If you’re already comfortable manipulating files and directories, searching for files with grep and find, and writing simple loops and 
scripts, you probably want to explore the next lesson: shell-extras.
# Download files

1. Download shell-lesson-data.zip and move the file to your Desktop.
2. Unzip/extract the file. Let your instructor know if you need help with this step. You should end up with a new folder called shell-lesson-data on your Desktop.


# Install software
If you do not already have the shell software installed, you will need to download and install it.

# Open a new shell

3. Open a terminal. If you’re not sure how to open a terminal on your operating system, see the instructions below.
1. In the terminal type cd then press the Return key. This step will make sure you start with your home folder as your working directory.

# Where to type commands: How to open a new shell

The shell is a program that enables us to send commands to the computer and receive output. It is also referred to as the terminal or command line.

Some computers include a default Unix Shell program. The steps below describe some methods for identifying and opening a Unix Shell program if you already have one installed. There are also options for identifying and downloading a Unix Shell program, a Linux/UNIX emulator, or a program to access a Unix Shell on a server.

If none of the options below address your circumstances, try an online search for: Unix shell [your computer model] [your operating system]

# The Shell

The shell is a program where users can type commands. With the shell, it’s possible to invoke complicated programs like climate modeling software or simple commands that create an empty directory with only one line of code. The most popular Unix shell is Bash (the Bourne Again SHell — so-called because it’s derived from a shell written by Stephen Bourne). Bash is the default shell on most modern implementations of Unix and in most packages that provide Unix-like tools for Windows. Note that ‘Git Bash’ is a piece of software that enables Windows users to use a Bash like interface when interacting with Git.

## Note that your prompt might look a little different. In particular, most popular shell environments by default put your user name and the host name before the $. Such a prompt might look like, e.g.:
 nelle@localhost $
## Command
$ ls
## Output
Desktop    Downloads     Music     Public          snap       Videos
Documents  frappe-bench  Pictures  site1.localRai  Templates

 ## If the shell can’t find a program whose name is the command you typed, it will print an error message such as:
 $ ks
 # Output
ks: command not found
## Command
$ pwd
## output
/home/hp
## Command
$ ls -F
## Output
Desktop/    Downloads/     Music/     Public/          snap/       Videos/
Documents/  frappe-bench/  Pictures/  site1.localRai/  Templates/

## Here, we can see that the home directory contains only sub-directories. Any names in the output that don’t have a classification symbol are files in the current working directory.

## Clear your terminal
$ clear

## Command
ls --help

## OUTPUT

```sh
Usage: ls [OPTION]... [FILE]...

List information about the FILEs (the current directory by default).

Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.

Mandatory arguments to long options are mandatory for short options too.

  -a, --all                  do not ignore entries starting with .
  -A, --almost-all           do not list implied . and ..
      --author               with -l, print the author of each file
  -b, --escape               print C-style escapes for nongraphic characters
      --block-size=SIZE      with -l, scale sizes by SIZE when printing them;
                               e.g., '--block-size=M'; see SIZE format below
  -B, --ignore-backups       do not list implied entries ending with ~
  -c                         with -lt: sort by, and show, ctime (time of last
                               modification of file status information);
                               with -l: show ctime and sort by name;
                               otherwise: sort by ctime, newest first
  -C                         list entries by columns
      --color[=WHEN]         colorize the output; WHEN can be 'always' (default
                               if omitted), 'auto', or 'never'; more info below
  -d, --directory            list directories themselves, not their contents
  -D, --dired                generate output designed for Emacs' dired mode
  -f                         do not sort, enable -aU, disable -ls --color
  -F, --classify             append indicator (one of */=>@|) to entries
      --file-type            likewise, except do not append '*'
      --format=WORD          across -x, commas -m, horizontal -x, long -l,
                               single-column -1, verbose -l, vertical -C
      --full-time            like -l --time-style=full-iso
  -g                         like -l, but do not list owner
      --group-directories-first
                             group directories before files;
                               can be augmented with a --sort option, but any
                               use of --sort=none (-U) disables grouping
  -G, --no-group             in a long listing, don't print group names
  -h, --human-readable       with -l and -s, print sizes like 1K 234M 2G etc.
      --si                   likewise, but use powers of 1000 not 1024
  -H, --dereference-command-line
                             follow symbolic links listed on the command line
      --dereference-command-line-symlink-to-dir
                             follow each command line symbolic link
                               that points to a directory
      --hide=PATTERN         do not list implied entries matching shell PATTERN
                               (overridden by -a or -A)
      --hyperlink[=WHEN]     hyperlink file names; WHEN can be 'always'
                               (default if omitted), 'auto', or 'never'
      --indicator-style=WORD  append indicator with style WORD to entry names:
                               none (default), slash (-p),
                               file-type (--file-type), classify (-F)
  -i, --inode                print the index number of each file
  -I, --ignore=PATTERN       do not list implied entries matching shell PATTERN
  -k, --kibibytes            default to 1024-byte blocks for disk usage;
                               used only with -s and per directory totals
  -l                         use a long listing format
  -L, --dereference          when showing file information for a symbolic
                               link, show information for the file the link
                               references rather than for the link itself
  -m                         fill width with a comma separated list of entries
  -n, --numeric-uid-gid      like -l, but list numeric user and group IDs
  -N, --literal              print entry names without quoting
  -o                         like -l, but do not list group information
  -p, --indicator-style=slash
                             append / indicator to directories
  -q, --hide-control-chars   print ? instead of nongraphic characters
      --show-control-chars   show nongraphic characters as-is (the default,
                               unless program is 'ls' and output is a terminal)
  -Q, --quote-name           enclose entry names in double quotes
      --quoting-style=WORD   use quoting style WORD for entry names:
                               literal, locale, shell, shell-always,
                               shell-escape, shell-escape-always, c, escape
                               (overrides QUOTING_STYLE environment variable)
  -r, --reverse              reverse order while sorting
  -R, --recursive            list subdirectories recursively
  -s, --size                 print the allocated size of each file, in blocks
  -S                         sort by file size, largest first
      --sort=WORD            sort by WORD instead of name: none (-U), size (-S),
                               time (-t), version (-v), extension (-X)
      --time=WORD            change the default of using modification times;
                               access time (-u): atime, access, use;
                               change time (-c): ctime, status;
                               birth time: birth, creation;
                             with -l, WORD determines which time to show;
                             with --sort=time, sort by WORD (newest first)
      --time-style=TIME_STYLE  time/date format with -l; see TIME_STYLE below
  -t                         sort by time, newest first; see --time
  -T, --tabsize=COLS         assume tab stops at each COLS instead of 8
  -u                         with -lt: sort by, and show, access time;
                               with -l: show access time and sort by name;
                               otherwise: sort by access time, newest first
  -U                         do not sort; list entries in directory order
  -v                         natural sort of (version) numbers within text
  -w, --width=COLS           set output width to COLS.  0 means no limit
  -x                         list entries by lines instead of by columns
  -X                         sort alphabetically by entry extension
  -Z, --context              print any security context of each file
  -1                         list one file per line.  Avoid '\n' with -q or -b
      --help     display this help and exit
      --version  output version information and exit
```
##  ls -t lists items by time of last change instead of alphabetically. 
 ls -t
## OUTPUT
Documents  Downloads     Desktop         Music     Public     Videos
snap       frappe-bench  site1.localRai  Pictures  Templates
## ls -r lists the contents of a directory in reverse order. 
ls -r
## Output
Videos     snap            Public    Music         Downloads  Desktop
Templates  site1.localRai  Pictures  frappe-bench  Documents
## Command
ls -F Desktop


## Output
'WhatsApp Image 2023-07-14 at 3.33.18 PM(2).jpeg'




