# Terminal Notes

Within a terminal you have what is known as a shell. This is a part of the operating system that defines how the terminal will behave and looks after running (or executing) commands for you. There are various shells available but the most common one is called bash which stands for Bourne again shell.

## reusing commands

When you enter commands, they are actually stored in a history. You can traverse this history using the up and down arrow keys. So don't bother re-typing out commands you have previously entered, you can usually just hit the up arrow a few times. You can also edit these commands using the left and right arrow keys to move the cursor where you want.

## navigating directories

pwd which stands for Print Working Directory
ls is a command to let you see your current directory contents
Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )
~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
. (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
.. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.
In order to move around in the system we use a command called cd which stands for change directory. If you run the command cd without any arguments then it will always take you back to your home directory.
Tab Completion
Typing out these paths can become tedious. If you're like me, you're also prone to making typos. The command line has a nice little mechanism to help us in this respect. It's called Tab Completion.

When you start typing a path (anywhere on the command line, you're not just limited to certain commands) you may hit the Tab key on your keyboard at any time which will invoke an auto complete action. 
Spaces in file and directory names are perfectly valid but we need to be a little careful with them. As you would remember, a space on the command line is how we seperate items. They are how we know what is the program name and can identify each command line argument. 

in order to use spaces for folder names you can use quotes using quotes around the entire item. You may use either single or double quotes or Another method is to use what is called an escape character, which is a backslash ( \ ). What the backslash does is escape (or nullify) the special meaning of the next character.

To make a file or directory hidden all you need to do is create the file or directory with it's name beginning with a . or rename it to be as such. Likewise you may rename a hidden file to remove the . and it will become unhidden. 

The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept. Some of them are a little hard to get your head around but they are fairly consistent in their structure so once you get the hang of it it's not too bad. You invoke the manual pages with the following command:

man <command to look up>

It is possible to do a keyword search on the Manual pages. This can be helpful if you're not quite sure of what command you may want to use but you know what you want to achieve. To be effective with this approach, you may need a few goes. It is not uncommon to find that a particular word exists in many manual pages.

man -k <search term>

man <command>
Look up the manual page for a particular command.
man -k <search term>
Do a keyword search for all manual pages containing the given search term.
/<term>
Within a manual page, perform a search for 'term'
n
After performing a search within a manual page, select the next found item.

reating a directory is pretty easy. The command we are after is mkdir which is short for Make Directory.

mkdir [options] <Directory>

The command to remove a directory is rmdir, short for remove directory.

rmdir [options] <Directory>

A lot of commands that involve manipulating data within a file have the nice feature that they will create a file automatically if we refer to it and it does not exist. In fact we can make use of this very characteristic to create blank files using the command touch.

touch [options] <filename>

Often before changing something, we may wish to create a duplicate so that if something goes wrong we can easily revert back to the original. The command we use for this is cp which stands for copy.

cp [options] <source> <destination>

To move a file we use the command mv which is short for move. It operates in a similar way to cp. One slight advantage is that we can move directories without having to provide the -r option.

mv [options] <source> <destination>

As with rmdir, removing a file is an action that may not be undone so be careful. The command to remove or delete a file is rm which stands for remove.

rm [options] <file>

mkdir
Make Directory - ie. Create a directory.
rmdir
Remove Directory - ie. Delete a directory.
touch
Create a blank file.
cp
Copy - ie. Copy a file or directory.
mv
Move - ie. Move a file or directory (can also be used to rename).
rm
Remove - ie. Delete a file.

Basic Navigation
pwd
Where am I in the system.
ls [path]
Perform a listing of the given path or your current directory.
Common options: -l, -h, -a
cd [path]
Change into the given path or into your home directory.
Path
A description of where a file or directory is on the filesystem.
Absolute Path
One beginning from the root of the file system (eg. /etc/sysconfig ).
Relative Path
One relative to where you currently are in the system (eg. Documents/music ).
~ (tilde)
Used in paths as a reference to your home directory (eg. ~/Documents ).
. (dot)
Used in paths as a reference to your current directory (eg. ./bin ).
.. (dot dot)
Used in paths as a reference to your current directories parent directory (eg. ../bin ).
TAB completion
Start typing and press TAB. The system will auto complete the path. Press TAB twice and it will show you your alternatives.
More About Files
file [path]
Find out what type of item a file or directory is.
Spaces in names
Put whole path in quotes ( " ) or a backslash ( \ ) in front of spaces.
Hidden files and directories
A name beginning with a . (dot) is considered hidden.
Permissions
r (read) w (write) x (execute)
Owner or User, Group and Others
ls -l [path]
View the permissions of a file or all items in a directory.
chmod <permissions> <path>
Change permissions. Permissions can be either shorthand (eg. 754) or longhand (eg. g+x).
Process Management
CTRL + C
Cancel the currently running process.
kill <process id>
Cancel the given process.
Include the option -9 to kill a stubborn process.
ps
Obtain a listing of processes and their id's.
Including the option aux will show all processes.
CTRL + Z
Pause the currently running process and put it in the background.
jobs
See a list of current processes in the background.
fg <job number>
Move the given process from the background to the foreground.
Manual Pages
man <command>
View the man page for a command.
man -k <search term>
Search for man pages containing the search term.
Press q to exit man pages
Vi / Vim
View our Vim Cheat sheet
Filters
head
Show the first n lines.
tail
Show the last n lines.
sort
Sort lines in a given way.
wc
How many words, characters and lines.
grep
Search for a given pattern.
See more on our Grep Cheat sheet
More filters can be found here.
Useful Commands
du -sh ./*
Find the size of every directory in your current directory.
df -h
Display how much disk space is used and also free.
basename -s .jpg -a *.jpg | xargs -n1 -i cp {}.jpg {}_original.jpg
Make a copy of every jpg image file in the current directory and rename adding _original.
find /home -mtime -1
Find all files in the given directory (and subdirectories) which have been modified in the last 24 hours.
shutdown -h now
Shutdown the system. (Replace -h with -r for reboot.)
File Manipulation
mkdir <directory name>
Create a directory
rmdir <directory name>
Remove a directory (only if empty).
touch <file name>
Create a blank file.
cp <source> <destination>
Copy the source file to the destination.
mv <source> <destination>
Move the source file to the destination.
May also be used to rename files or directories.
rm <path>
Remove a file or directory.
Common options: -r -f
Wildcards
May be used anywhere in any path.
*
Zero or more characters (eg. b*).
?
Single character (eg. file.???).
[ ]
Range (eg. b[aio]t).
Piping and Redirection
>
Redirect STDOUT to a file.
>>
Append STDOUT to the end of a file.
2>
Redirect the STDERR to a file.
<
Pass the contents of a file to a program as STDIN.
|
Feed the STDOUT of the program on the left as STDIN to the program on the right.
