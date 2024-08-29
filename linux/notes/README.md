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

    

    



    

  
   
  


