# Module 1: LINUX!!
Learning Objective: Understand The Linux File System, Command Line Interface, Process Management and Common Linux Tools.

What Is Linux?

Linux is an Open Source Operating System (THIS MEANS THAT IT IS LIKE A COMPUTER SOFTWARE THATS OPEN TO EVERYONE TO SEE, USE AND MODIFY.) 
Important Note For Explanation In Interviews If Asked: Linux is a popular and efficient operating system because it is known for its security, flexibility and strong community support, it is cost effective and highly secure making it the go to operating system used in Tech Companies:)
Linux is the backnone of many Servers Networks and Cloud Infrascructures 
Versions of Linux is known as Distributions or 'Flavours'

INTRO TO LINUX COMMANDS!!!

pwd - 'Print Working Directory' : This Command Tells You What Directory you are in... For E.g if you are in your Desktop Directory and you run in the command 'pwd' in the terminal, it would say something like '/Desktop/'

cd - 'Change Directory' : This Command Allows You To Go To A Different Directory... For E.g if you are currently in your Desktop directory and you put in the command 'cd' in the terminal, it will automatically take you out of your Desktop Directory... Another Example is that if you want to go from your Desktop Directory to your Downloads, you would put in the command 'cd Downloads'.

mkdir - 'Make Directory' : This Allows You To Create New Directories (Another word for Directory Can Be Folder) For E.g if you wanted to make a folder called 'My Work', you would run the command 'mkdir my Work' in the terminal and it will create a folder called 'My Work'.

rmdir - 'Remove Directory' : This Command Allows You To Remove Directories (Folders) that you have made...For E.g if you wanted to remove the 'My Work' Directory that you made, you can simply use the the command 'rmdir My Work' and the folder will be removed 

touch - This Command Allows You To Create Files (whether thats in Directories or not)... For E.g if you where already in your Desktop Directory and you wanted to make a file within it called 'Tech Summaries' you can use the command 'touch Tech Summaries'

rm - This Command Allows you to Remove Files you have created...E.g if you wanted to remove the file 'Tech Summaries' in your Desktop directory, you can run the command 'rm Tech Summaries'

TOP LINUX COMMAND SUMMARY!!!
pwd- 'Print Working Directory'
cd- 'Change Directory'
mkdir- 'Make Directory'
rmdir- 'Remove Directory'
touch- 'Make File'
rm- 'Remove File'

What Are Linux Commands?

Linux Commands are what is known as 'Texual Instructions' that tell the Operating System what to do!!
Linux Commands can be enetered directly into the Terminal
Linux Commands are 'Case Sensitive' For E.g the Linux Command 'ls' must be in lower case, otherwise the OS may take it as another command.

IMPORTANT NOTE: Linux Commands have various 'Options' and 'arguments' that modify their behaviour... For E.g
The Linux Command 'ls' on its own means 'Listing Contents'
However 'ls -a' means listing contents but even the hidden ones 'a=all' = Hidden Files and Directories 'ls -a.' also refer to hidden files beggining with '.'

IMPORTANT: Linux Commands - Manual Page 

What is the 'Manual Page' and its importance?

Manual Page: a page in the terminal that tells you how to use a command as well as what options and arguments it has. The Manual Page also tells you what a command does.

How to access the manual page of a command in the terminal:

The 'man' command allows you to open up the manual for the command you want to use... For E.g 'man ls'...This will tell you how to use the 'ls' command as well as the options and arguments it has. 

NOTE: any directories or files that start with a '.' are hidden files and are ignored by the 'ls' command which is why 'ls -a' is an option as we previously discussed.

The command: 'man man' tells you how to use the 'man command' (its like the manual for the manual command)

EXPLORING THE 'man' COMMAND WITH DIFFERENT COMMANDS!!!

NAME: mkdir - 'man mkdir' : opens up the manual for the mkdir command 
As we already know - 'mkdir' on its own - "make directory"

mkdir -m / mkdir --mode:

"Set File Mode" - This Option for the 'mkdir' command '-m / --mode' is used to specify the "Permissions" that the newly created directory should have.
                                             E.g
'mkdir -m 755' would create the directory mode that will be named 'my directory' with the permission mode '755'. This means that the owner has full permissions of the directory meaning they have full acces to view and edit contents inside of it. Depending on the permission settings you require, the ' -m / --mode' can set the directory to it 

mkdir -p / mkdir --parents:

"This Option allows you to create a directory and any necessary parent directories that do not exist"

                                            IN SIMPLE TERMS
When you use the 'mkdir -p' Option, its like a shortcute that helps create not just one folder but also any other folders that need to be made to reach that main folder.

NOTE: A parent directory is the main folder that holds other folders and files inside of it.

mkdir -v / mkdir --verbose

"print a message for each created directory" 

when using the 'mkdir -v' Option, it makes the mkdir command show you a message for each directory it creates!

Its like the command is talking back to you, letting you know exactly what its doing as it creates directories 
                                                  E.g
If you use the command 'mkdir -v my folder' the command will create a folder named "my folder" and then show a message like "mkdir created directory "my folder" to confirm that the folder was created.                                                  





INTERESTING COMMANDS!!!

What Are Head And Tail Commands?

Head and Tail commands are useful for viewing the beggining and end of files.

Lets say for example you have a massive file, and you dont want to use the cat command to list the contents within the file because its just too long!

Head and Tail command are helpful when you are dealing with particulary large files and only want to view the beggining and end of the files!!

What is the head command?

The head command allows us to view the first '10 lines' of a file.

So lets say for an example, you have a file that has 20 lines, but you only want to view the first few lines of the file...The 'head' command will display the first 10 lines of the file!!

Now lets say that you want to specify a number of files that you want to view... you would need to add an arguement/option to do this 

VERY IMPORTANT EXAMPLE!!

So if you want to soecify the number of lines you want to see in the file, you run the command:

"head -n (whatever number you want) 'filename.txt'"

The "-n" allows you to choose the number of lines in the files that you want to access.

Lets say that you had a file called 'multiline.txt' and within this file you have 20 lines bhut you want to view the first 4 lines of the file, You would run the command:

"head -n '4' multiline.txt"
                                                                   The terminal should then list the first 4 lines of this file!!!
                                                                   Now, In Contrary...
                                                                   The Tail command allows you to view the last 10 lines of a file!!
                                                                   So lets demonstrate another example...
                                                                   if you had a file called multiline.txt that had 20 lines and you wanted to view the last ten... You would run the command...
                                                                   'tail multiline.txt'
                                                                   This will display the last 10 lines in the file to be precise!!
                                                                   Now lets go through another example!!
                                                                   Lets say that you wangt to view the last 7 lines of a file...
                                                                   What command do you run??
                                                                   'tail -n 7 multiline.txt'
                                                                   This will display the last 7 lines of the the file!!
                                                                   Remember the '-n' option lets you choose which number you want to select the number you want!!!
                                                                   Did you know that you can use the 'Head' and 'Tail' commands together to view specific scetions of a file??
                                                                   Lets say you wanted to view lines '6 to 10' of a file, the 'Head' command will not directly give you these specifications because it only lists the first 10, which means that you would need to run the tail command along side it to display the correct answer...
                                                                   Lets take a look at this further!!!
                                                                   The first thing you would need to do is to list the first 10 lines of the command, like this...
                                                                   'head -n 10'
                                                                   REMEMBER!! The '-n 10' option in this scenario is not necessary since the 'head' command already does this, however we need to specify it to complete the next part of the command!!
                                                                   Then we use what is known as the '|' "pipe symbol" and then you add the file name after it (in this case multiline.txt) following with completing the command with 'tail -n 5'
                                                                   So the whole command should look something like this:
        

             head -n 10 multiline.txt | tail -n 5
                                                                                             
A Summary of what we are telling our linux file system!!

Weare telling our linux file system that we want to find the first ten lines of our file,'multiline.txt' and once we've done that, we want to print the last 5 lines of those ten lines which is initially 6-10!!!

what is this character '|' (pipe symbol) doing in this command???

the '|' pipe is passing the contents of the first command as an arguement to the second command!!

SUMMARY!!
The 'Head' AND 'Tail' commands are powerful tools for quicly viewing the begining and ending of files, by specifying the number of libes to display, you can easily inspect different parts of a file without needing to open the entire file!!!
                                                                  QUICK NOTE:

The 'Vim' command is a text editor command that allows you to edit files, similar to the 'nano' command

All about File Management commands!!!

what are file management commands?

3 essential file managemnt commands

'cp' 'mv' 'rm'

the 'cp' command allows you to copy files and directories

Lets say if you want to copy a file you made! we previously made a file called 'multiline.txt' so we will use this for our example! 

if you want to copy the 'multiline.txt' file into another file such as 'multiline_copy.txt' for example 

you run the command:

'cp multiline.txt multiline_copy.txt'

This command coppied 'multiline.txt' into the 'multiline_copy.txt'file!!

you can also use the 'cp' command to copy a directory as well as a file, but you have to use the '-r' option as an arguement!! so it will look something like this "cp -r"

This is because the 'cp' command by default does not copy directories so we have to use the '-r' arguement

The '-r' option stands for recursive

Lets show an example!!

if you had a directory called 'my work_ubuntu' for example and you wanted to copy it, you would run the command:

'cp-r my work_ubuntu my work_ubuntu_copy'

 Lets break it down!!

 you are copying your already current directory that you have made which is why you have to as the '_copy' addition becayse then it officially becomes a copy of the current directory.

 rm and mv Commands in More detail!!

the 'mv' command isn used to move or Rename files 

Lets demonstrate how the the 'mv' command Renames files!!
Lets say that we wanted to Rename one one of our files, in this case we can use the example 'multiline_copy.txt'

Remember that this is the file that we copied with the 'cp -r' command.

using the 'mv' command we can rename 'multiline_copy.txt

It should look something like this:

' mv multiline_copy multiline_backup.txt '
if you want to move a file to a different directory, you can use the 'mv' command like this 
'mv 'examplefile.txt' 'example_directory'

what about the 'rm' command?

The 'rm' command is used to move both files and directories!!

lets say you wanted to remove a file within a directory.

so we have 'examplefile.txt' within the directory 'examplefirectory' to remove this file from this directory we would run the command 

'rm examplefile.txt'

REMEMBER!! YOU NEED TO NAVIGATE TO THE DIRECTORY 'exampledirectory' dor un the command above first.

Then if you run the command 'ls' the 'examplefile.txr' should be removed from the 'exampledirectory'

now if we want to use the 'rm' to remove a directory 

you have to use the '-r' option

so lets say you want to remove the directory 'exampledirectory'

you would have to run the command:

' rm -r exampledirectory '

Then when you enter the 'ls' command the the directory should not come up on the list 


mkdir command notes aaddition:

- you can make nested directories with the mkdir command
- nested directories are like folders within folders (for context)
- you cannot create nested directories with the 'mkdir' command alone
- use 'mkdir -p' to make nested directories (folders within folders)
- use the 'ls -R' command to view nested directories
- the '-R' option lists directories recursively meaning to list contents withhin directories that are also withi other directories
- 'rmdir' can only remove empty directories
- 'rm -r' removes contents from directories as well as directories themselves

  Dealing with tricky spaces in folder names!!!:

- spaces in folder names can cause issues due to the system recognising the 2 segregated words as different directories
- to create a project with spaces in it... use speech marks e.g 'mkdir "My Project"'
- This will make a directory called 'My Project'
- another approach: use the '/' character E.g 'mkdir My\ Project\ 2'
- this will make a directory called 'My Project 2'
- How to navigate to directories with spaced in them? use the 'cd' command followed by speech marks and having the directory name inside them e.g 'cd "My Project"

Vim Text Editor!!!
-Vim is widely used because ofits efficiency and extensive feature set
- the 'vim' command will create afile for you if it doesnt already exist like the 'echo' command
- to edit a file, run: 'vim examplefile.txt'
- The 3 most important modes of the 'vim' command:
- 1. command mode: allows you to move around in file and perform
     various operations like deleting text
     
how to navigate command mode: use 'h' to move left accross text, 'j' to move down, 'k' to move up, 'l' to move right

to save changed, you need to be in command mode and type ':wq!'
     
  3. insert mode: where you can insert and edit text
  4. Visual mode: you can use to select text in a visual format
  - to navigate between modes you need to press the 'Esc'
  - if you do not want to save changed in the command mode you type ':q!'

    VIM Navigation!!! (very important!!)
    
- to move to the beggining of the line in vim editor press '0'
- and to move to the end pf line press '*' or shift + 4
- moving forward press 'w'
- Move backwards by pressing 'b'
- to go to a specific line type ':' following up with the line number you need
- to search for a word in the text if its too long, stay in command mode and type'/' following what what you want to search for (occurance)
- if you want to look for a second occurance (the same word but in a different line, you navigate this pressing 'n' and if you want to go back to the first occurance (first word of the same word that you searched) you press 'N'
- if you want to delete lines in the vim text editor, you navigate to the line you want to delete and press 'dd'
- if you want to just delete from the middle of the line to the end, you would navigate from the middle of the line and press 'D'
- copying is known as 'yank' in vim and to do this you need to navigate to the line you want to copy and press 'y' then to paste the copies text, you press 'p'
- to undo changes in vim press 'u'
- to redo undone change you press 'ctrl + R'
- Vim enables syntax highlighting which makes it easier to read configuration files
- to enable syntax hyghlighting with vim type ':syntax'
- to view the numbers of of files type ':set number' In command mode and to remove number 'set nonumber'
- ':w' is just to save work in vim, it will not exit out the file
- ':wq!' forces vim to save and exit file 

    The 'sudo' command!!

  - the 'sudo' command stands for 'super user do'
  - this command allows a permitted user to execute a command as the root user
  - you have to be a permitted user to use the 'sudo' command
  - example of sudo command 'sudo apt-get install'
  - some commands can only be run by the root user or a user that has elevated permissions, these include commands that allow you to install a package or update 
  - an example of a command where you will need a root user or elevated permissions is the 'apt-get' command
  - if you run this command without 'sudo' your access will be denied
  - to run the previous command, you can add '!!'
  - editing configurtion files also need a user permission or a root user
- to edit configuration files, you need to enter the 'sudo' command to be granted access to edit them for example 'sudo vim /etc/nginx


  The Root User and Dangerous commands!!!
  
- you might need to navigate to the route user to perform administerative tasks
- to enter your route user, run the command 'sudo su'
- you might want to use this if you are using multiple commands that require super user permissions
- the 'whoami' command can verify what user you are using
- there are dangerous commands you can runas a routr user
- As a root user you have unrestricted access to the whole system
- to return to normal user type 'exit'
- EXTREMELY DANGEROUS COMMAND: 'rm -rf /'
- This command is telling the system t remove everything on it which means you will loose all files and directories
- all sudo commands are logged for security purposes
- you can view the sudo log entaries in a file called '/var/logauth.log
- if you run the command 'sudo tail /var/logauth.log' it will show you the last ten lines of the file and show all thetimes youve used the 'sudo command' 

  Users in Linux!!
- This section  will teach you how to create a user, switch users, add and remove users from the sudo's list, and verify sudo access
- command to create a new user: 'sudo useradd newuser'
-  command for creating password for new user: 'sudo passwd newuser'
- command for switching user: 'su - newuser'
- run the 'whoami' to display the username associated with the current user who is logged
-   to add your new user to the priviledges list or 'sudo's' list to be able to run commands that require higher acces in the user: run the command: 'sudo usermod -aG sudo newuser'
-   Command that allows you to read the contents of the root directory: 'sudo ls /root'
- without 'sudo' the command above cannot work
-  to remove your user from the priviledges list, run the command: 'sudo deluser newuser sudo'
-  

    Groups in linux!!
- to view all the groups inside your linux system, run the command: cat /etc/group
-  if you want to create a new group in your linux system, run the command: 'sudo groupadd 'whatever group name'
-   To add a new user to your new group, you can run the command: 'sudo usermod -aG 'group name' 'username you want'
-   the 'group' command lists all the groups that the user is in
-   to remove a user from a group, you run the command: 'sudo gpasswd -d 'username' 'group' name
-  command for deleting groups: sudo groupdel 'group name'
-  users can be belong to multiple groups which can be usefull for managing permissions and access
-  how to add a user to a group: 'sudo usermod -aG 'group you want to add too'
-  group management is crucial for controlling uder permissions
  
  
  Introduction to file permissions
  - 'ls -l' is the command we can use to view file permissions
  - file permissions control who can read, write or execute a file
  - file permissions may look something like this 'rwx' which stands for 'read, write and execute'
  - 'write' means you can modify the file or edit it and 'x means you can run the file as a program
  - permissions are assigned to 3 catergories withtin the linux system... 'user category, 'group catergory' and 'other'
  - the 'user' is the owner of files and who you are currently logged in as, the 'group' is a group of users with the same permisions and 'others' represent other users...'everyone else'
- for example if i was to create a file using my ubuntu user and you have specific permissions for the file where everyone else cannot read and write or execute on it (rwx) means that if you was to switch to a newuser and try and edit the file, you would not be able to because the new user does not have the correct permissions to do so
- maintaining file permissions is vital for maintaining security on your system


  Binary, Octal and string Representation!!
  summarised notes
- permissions representation can be represesnted in a binary format
- binary format is when permissions is represented as binary digits
- Binary is a set of digits, represented by '0' and '1' that have base 2
- Octal prepresentation: compiled representation using numbers
- Depending on what permissions has been set also depends on the binary representation, for example, if you have permissions set to 'r-x' this means that you are able to read the file as well as execute the file as a command but cannot modify or edit the file.
- the binary representation for this permission would be '101' because 2 permissions are on and the other is off 'r-x'
- another example permission 'rw-' which means the user cannot execute the file as a command but can read and modify/edit the file
-   with the octal representation, number '7' means that the user has been given all permissions, number '6' means that you have only 2 permisions and number '5' meand that you have 2 permissions but not the middle one so it weights less

- permission settings of a file can look like this: '-rwxrw-rw-' this means for example a files user has the permissions to read, modify and execute file, groups have permissions to read and modify the file only and others can read and write in the file aswell

-   visual example: 'rwx' - 7(4+2+1)
-                   'rw-' - 6(4+2+0)
-                   'r-x' - 5(4+0+1)

  chmod calculator allows you to set permissions for the 'owner' 'groups' and 'public' so you can play around with the permissions and see which permissions

chmod Command: Symbolic and Numeric representations!!

- the 'chmod' commands allows us to change the permissions of a file or directory
- there are to different ways to represent the 'chmod' permissions called 'numeric' and 'symbolic'
- The symbolic representation is using the 'chmod' command with the 'ugo' which stands for 'user' 'group' and 'category' following with the letters 'rwx' that we dealt with before.

- symbolic file permissions use these letters 'rwx' to represent the permissions for the 'ugo' user, group and others.
- Heres and example of how you would grant the user execute permissions for a file, grant the group read permissions for a file and takeaway the write permissions from others for the file, using symbolic represenation of 'chmod':

  'chmod u+x,g+r,o-w 'filename.txt'

   - Numeric file permissions use numbers to represent the different permissions, this is the octal representation that we went through before
   - each permission 'rwx' has a corresponding value e.g 'r=4' 'w=2' 'x=1' this is why, when you want to give full permissions, you would use the value '7' in numeric representation of 'chmod' and limited permissions with others or groups using '5' or '4'
   - example command 'chmod 750 'filename.txt': this permission settings mean that you are giving the 'user' full permissions, 'groups' only read and execute permissions and 'others' no
 permissions

  what are scripts?
  - Scrips are executable files that you can run as a program
  - so what you do is give a set of commands in a script which you can then use as a program
  -  to run files that are scrips, all you need to do is type './' followed by the file you want to execute E.g ' ./examplepermissionsscript '
  - if you want to give execution permissions to a permissions file script, run the command  'chmod +x 'examplepermissionsscript'

- if you want to specify permissions to both 'user, groups' you can add the '=' character sign to specify both at the same time E.g 'chmod ug=rw o=r 'examplefile.txt'

  Changing file/Dir ownership for User/group!

  - To change the owner of a file or directory we use the command 'chown', but we have to use the 'sudo' command before using 'chown' because this command is used for users who have permission or access only!

     Using the 'Chown' (change owner) command may look something like: 'sudo chown 'new user' 'name of file you want to change it to'

to change groups of a file or directory we use the command 'chgrp' this command also needs 'sudo' infront of it before it can run.

  Using the 'chgrp' (change group) command may look like this: 'sudo chgrp 'new group' 'name of file you want to to make the change of group to.

- you can change both the owner and group of a file AT THE SAME TIME using the 'chown' command which is tim efficient and easier
- ' sudo chown "name of group you want to change to":"name of user you want to change to" "name of file you want this command to effect"

  E.g 'sudo chown ubuntu:admin2 example.txt'

  - to change the ownership of a direcory you have to run the 'chown' command followed by the '-R' option (recursive)

    Example command: 'sudo chown -R "name of user and group you want to change to" 'name of directory you are directing changes to'

    E.g 'sudo chown -R newuser:admin2 myworkingdirectory'


    Introduction to standard streams: Data redirection section
    
- in linux, understanding standard streams is crucial for handling input and output effectively
- THERE ARE 3 STANDARDS STREAMS

1. Standard Input Stream: This is the stream that provides input to commands
   ( when you type a command in your keyboard and then its past into the running program or linux file system) it could also be redirected from a file for example: when you type in a command and 'press enter' you are using standard input

2. Standard Output: is the stream where commands send their out put onto the screen, for example if you type '$echo SHELL' and the terminal prints 'bash' that is the output of the linux file system followed fromthe command you inputed in.

   3. Standard Error: standard error display's errors on the terminal so that you can actually see when you make an error, for example if a command fails the error message is sent through 'standard error'

Managing these streams effectively allows you to control how input and output are handled in your scripts and commands.


      
    
    

    

    

- 
  

  


    

  
   
  


