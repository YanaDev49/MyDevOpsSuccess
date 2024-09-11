In order to create a Bash Script, You need to Open a file using the 'touch' command

E.g touch examplescript.sh (Make sure you add '.sh' at the end of Bash Scripting files to allow the terminal
to Recognise that this file will be executed)

You can edit your bash scripting file using any text editor command for example 'vim' or 'nano'

                      E.g 'vim examplescript.sh'

How to edit your Bash Script using the 'vim' command?

start by pressing 'i' in the 'vim' command to enter '---INSERT---' 

Note: The first line of every Bash Script should begin with with a Shebang line, which looks like this '#!/bin/bash'

So what is a Shebang line?

The shebang line tells your computer to run the Script using bash!
It specifies which interpreter we will use when running the script 

How to add text to your Bash Scripting!!

After you have established the #shebang line, you can start adding text to your file by 
using the 'echo' command followed by the text you want to add.

                       E.g 'echo "Hello everyone"'

Remember to exit ---INSERT--- using the 'Esc' button on your keyboard, and once you 
enter command mode, type 'wq!' to save your changes 

Note: Due to the fact that your bash scripting file is an executable file, you need 
to grant it permissions using the 'chmod' command!

          E.g 'chmod +x examplebashscriptfile.sh'

After youve granted the file permissions, you can execute the file using './'

                      E.g ./examplebashscript.sh

(the script should show up on the terminal)

Note: Did you know that you can actually run your bash script without using './'

Thats Right!! 

there are 2 other ways in which you can run your bash script, using the 'sh' command
and the 'bash' command

              E.g ' sh examplebashscript.sh '
                             or
                ' bash examplebashscript.sh ' (These commands are for when you dont specify
  the interpreter in the bash scripts... This isfor when you dont use the shebang line)

Note: the shebang line is not just limited to the bash shell, you can use different interpreters
according to your needs and by specifying the correct interpreter in the shebang you can ensure that
your scripts are executed consistently regardless of which shell or enviroment you are running.

QUICK SUMMARY!!

- The shebang Line starts with the #!, it specifies the interpreter or shell that should handle the script
- it enables consistent executable scripts accross different enviroments, regardless of what shell you are using
- you can specify different interpreters for different scripts
- the shebang line should be the very first line of your bash script

COMMENTS IN BASH SCRIPTING!!

- Comments enhance clarity and understandibility of a script
- comments are lines in a script that are not executed as part of the code 
- comments explain what the code is doing and provides an explanation for the steps in the code
- Adding comments to your script is considered best practices because it helps you and others understand
whats going on in the code which provides clarity and logic of the script


To add comments to your bash script you have to add '#' followed by the the comment that 
you want to put 

        E.g '#We are renaming this file'

There are also multi-line comments in bash scripting that are made using ": and '"
you begin your multi-line comment with ":'" to the amount of lines you want to extend the comment to and close 
it with "'"

            E.g " : 'The cp command in this script will copy this text in the next 
                   file' "

When you run a script, comments will not show, however when you run the cat command,
it will show you the contents within the file without running the file as a script
and will display the comments that youve added into the file. This is because, reviewing the contents within 
a file is not the same as running the script itself.

This is why comments do not show when you run the script

- comments are useful for individuals who are new to bash scripting as they explain 
what the code does in the file which provides logic and clarity as mentioned 

Interesting ways to use comments in bash scripting!!

if you want to prevent a script from running in bash scripting, you can turn the lines in a 
script into a comment if you want to prevent it from running by adding '#'

If you try run the bash script, the lines that you have turned into comments will not run


How to run your script in anywhere without specifying its path!!

Note: you need to place your script in one of the directories in your PATH ENVIROMENT VARIABLE

(Remember, this is the enviroment variable that contains all the programs to run the commands you input)

- you need to add your script to the /usr/local/bin using the command:

         ' sudo mv examplebashscriptfile.sh /usr/local/bin/examplebashscript.sh '

After this, you need to grant your script permissions to run the script and from any path using the:

'sudo chmod +x /usr/local/bin/examplebashscript.sh' (we need to grant this permissions to enable the files execution from any enviroment'

Now you can navigate to any directory and still run the script... E.g if you navigate to your desktop directory 
and you want to run your bashscript, you can simply type 'examplebashscript.sh' (Remember, you have to type the name of the file YOUR bashscript is saved as)
and press enter and it should run the script.


Variables in Bashcripting!!

Variables are an essential component of bashscripting as they allow you to store and manipulate data 
and makes your script flexible

- variables are created using the assignmnet operator '='

                  E.g greeting="Hello world!'

- To access the value of a variable, you have to put a '$' in front of the name of 
the variable.

                    E.g echo $greeting

This means that if you run the echo command following the '$' and the variable 
it will run the value of the variable 



                 E.g greeting="Hello world!"

                   echo $greeting 

                      Will Run

                  echo "Hello world!"


- Variables can hold different types of data for E.g: strings, numbers and arrays

                         EXAMPLES!!

Strings: (Text)  greeting= "Hello Everyone!"

Numbers: (integers) count= 43

Arrays: (()) fruits= ("apples", "bananas", "pears")



Parameters in bash scripting!!

- Parameters allow you to customize the behaviour of your script and make it more flexible!!
- parameters are input values from the command line when they are executed 

-Parameters allow you to input a variable that will show up on your bashscript

           E.g echo "Parameter 1: $1"
               echo "Parameter 2: $2"
               echo "Parameter 3: $3"

This means that you can customise the variables '$1 $2 $3' youve entered after 
the parameters on the terminal and make the output of the script whatever variables
you would like.

  For example, when you want to run the script you simply:

             ' ./examplebashcript Hello world

                 Parameter 1: Hello
                 Parameter 2: world
                 Parameter 3:                 '

As you can see, we have controlled the variables that we have entered into our script
using parameters!!


what if we wanted to access all the parameters into a script?

open your '.sh' for example 'examplebashscript.sh' 

and add in the command ' echo "All Parameters: $@"

This means that when you run the script, for example: 

        ./example bashcript hello everyone world

        Parameter 1: hello
        Parameter 2: everyone
        Parameter 3: world
        All Parameters: hello everyone world
          
(This will be the output)


Arithmetic Expansion In Bash Scripting!!

- Bah Provides a straight forward way to perform mathmatical calculations and evaluate
expressions using '$(())' = dollar and paranthesis notation 

with '$(())' we can perform arithmetic calculations within our bashScript 

An example bash script using dollar and paranthesis notation:

' #!/bin/bash

num1=6
num2=4

result=$((num1 + num2)) --------> This is how we use the dolla and paranthesis notation


echo "The sum of $num1 and $num2 is: $result '


RESULT OF CODE: 


' Run Code- ./calculation.sh (this is the file that i have made for my script)

The sum of 6 and 4 is: 10 '



A MORE TECHNICAL SCRIPT USING $(())

'length=10
 width=16

area=$((length * width ))
perimeter=$((2 * (length + width)))

echo "Rectangle area: $area"
echo "Rectangle perimeter: $perimeter" '

RESULT OF CODE:

'  ./Area.sh
Rectangle area: 160
Rectangle perimeter: 52 '


Arithmetic parameters



The 'if statement' in bash scripting 

- if statements allow you to include decision making logic into your script executing different code blocks
based on specefic conditions 

- They provide a way to control the flow of your bashscripts, they allow you to evaluate conditions
and execute different code blocks, based on the result

- They enable you to make decisions and create dynamic behaviour in your scripts

- conditions in if statements are formed using comparison operators E.g:

eq = equals
ne = not equal to 
lt = less than 
gt = greater than
le = less than or equal to 
ge = greater than or equal to 

- if statements become even more powerful with logical operators




LOGICAL OPERATORS LOOK LIKE THIS:

&& = AND 
|| = OR

This means that if you want to create more complex conditions using the AND or OR logical
operators you can in your bashscript 


String comparisons in bashscripting!

== - equal to 
!= - not equal to 


The 'else' and 'elif' statement

- The else clause provides a code block alternative to be executed when the 'if' condition turns out to be false.
- 'elif' allows us to add another 'if' statement or condition is the first condition is false

Example:

price=35

if [ $price -gt 25 ]; then
    echo "your budget is just right!" 
elif [ $price -gt 25 ] && [ $price -lt 75 ]; then 
    echo "your budget is just right:)"
else 
    echo "Sorry, your budget is invalid"
fi


what are nested 'if' statements?

-nested if statements allow us to create more complex decision making structures by imbedding 'if statemensts' into other 'if statements'

example: age=34
grade=65

if [ $age -ge 25 ]; then 
    echo "you are elegible for this programme based on your age"
    if [ $grade -ge 90 ]; then
	    echo "your grade is elegible for this programme!"

   else 
        echo "Sorry you are not elegible for this programme!"

    fi 
else
        echo "Sorry, your grade is not elegible for this programme"

fi '


While loops in bash scripting!!

- while loops allow you to repeatedly execute a block of code as long as a condition
is true 
- the condition is evaluated before each iteration 
-the loop continues until the condition becomes false 
- its important to note that while loops are useful for automating tasks and iterating other data 

Example: 'count=1

if [ $count -eq 1 ]; then
    while [ $count -le 20 ]; do 
        echo "Count: $count"
        ((count++))
    done
else
    echo "Sorry, cannot execute"
fi'



For Loops in bash scripting!!

for loops allow you to repeat a block of code for a specified number of iterations or over a sequence of values 
they are a powerful tool for automating operations and helping you to perform repetitive tasks and processing data



Break and Continue statements in bash scripting!!

- break and continue statements allow additional control within for and while loops
- this allows you to interupt or skip while loops based on specific conditions
- they give you the flexibility to interrupt a loop or skip iterations if necessary.

- The continue statement allows you to skip the rest of the current iteration and move on to the next iteration of the loop

Summary
- The break statement exits the inner most loop it is placed in  
- The continue statement skips the most current iteration for the loop and moves on to the next iteration  
- both break and continue statements can be used with for and while loops to fine tune the behaviour of loops 



Basics of functions in bash scripting!!

- functions allow us to turn our code into modules 
- improves script organisation 
- enhances re-usability
- functions are like mini programs within our bash script 
- they encapsulate a set of instructions which are called and executed whenever needed


Parameters in bash scripting!
- There are 2 types of parameters, positional parameters and  special parameters
- parameters allow us to pass data to functions making them more versatile and adaptable
- function parameters provide a way to pass data to functions enabling them to perform specific tasks based on provided inputs 
- positional parameters allow us to pass data to functions and access them using numbered variables like '$1' and '$2'
- special parameters provide additional information about the scripts and the arguements passed to it

such as: '$#' = which tells you the number of arguements 
         '$0' =  tells you the name of the script
         '$1' = tells you the first arguement you inputed 
         '$2' = tells you the second arguement you inputed 
         '$@' = tells you all arguments 

User inputs in bash scripting!!

- user input allows our scripts to interact with the users and make them more dynamic and make them more responsive 
- by using user inputs, we can create powerful and interactive scripts 
- using the 'read' command, the script can allow the user  to input anything they want, example 'read_name'
- The read command is useful for interactive prompts, allowing users to enter information in the script  
- command line arguements provide a direct way to pass direct user input when calling user functions

Handling bad data in bash scripting!!

- bad data refers to invalid or unexpected user inputs which may cause errors or undesired behaviours in our scripts
- by implementing proper error handling techniques we can ensure that our scripts gracefully handle data 
and provide informative feedback for the user
- conditional statements can be used to handle 

Piping in bash scripting 

- piping allows us to pass an output of one command as input to another using the '|' symbol 
- this allows us to connect commands and pass the output of one command as input to another 
- piping within functions enables to perform advanced data operations and store the results in variables
- we can combine piping with other commands or functions to create more complex data manipulation pipelines 

Introduction to error handling!!

- error handling in scrips is about forseeing where things can go wrong and taking the appropriate measures to handle those situation  
- effective error handling can make your scripts more reliable and trust worthy and is considered best practice


if statement Recap for error handling i bash scripting!

-

Exit Codes For bashscripting!

- whenever a command or script ends, it returns an exit code to the system
- this is a numerical value indicating if the script ran succsessfully or not 
- an exit code of 0 = success and an exit code of any other number is not a succesess, indicates an error

- when we run a command and it is successful, its exit code is 0 which means that it has passed through to the system, if a command fails its exit code will be another number which means its an error

TO CHECK THE EXIT CODE OF THE PREVIOUS COMMAND RUN, RUN THE COMMAND:
'echo $?'


set -e in Bash Scripting!!

# The 'set -e command' will tell the script to stop running if an error occurs 
# using 'set -e' command can help us catch errors as soon as they happen
# This avoids unexpected behaviour in the scripts 
# its important to understand that not all exit codes that are not = to zero are errors
# sometimes you may want to run your script even with an error and in this case you will not add 'set -e'

set -u in Bash Scripting!!

#The 'set -u' stops the script if it encounters an un initialised variable in the script
#This means that if we have used a variable in the script that has not been created in the first place 
#in this script we have told the system to execute the value of a variable that deosnt exist e.g 'variable X: $X'
#the 'set -u' command stops the script if an unidentifiable variable has been executed

#In this script we are using arithmetic expansion to solve an eqaution of numbered variables 
#Although this is the case there is one uninitialised variable in the equation which means that it does not exists, we have not initialised the 'W' variable
#the 'set -u' command will stop the script because the uninitialised variable will be noticed by the 'set -u' command and stop the script

set -x and set +x in Bash Scripting!!

# a powerful tool for debgugging in bash scripts is the 'set -x' command
# the 'set -x' options prints each command that will be executed to the terminal before it is actually executed 
# The 'set -x' option prints out all the values you have inputed into the script along with its commands to show you what it is doing
# This shows you precisely each step in execution showing how the script is proceeding 
#The 'set -u' option is very useful for troubleshooting scripts
#if you only want to debug one part of your script you can put the option 'set +X' to allow the rest of your script to carry on as normal


set -eux in Bash Scripting!!

- Bash allows us to use the 'set -e, set -u, set -x' all in one go to maximize the debugging process
- the 'set -eux' option will stop the script because of the error because of the 'e' flag, will stop the script because of an uninitialised variable due to the 'u' flag
and will print each command before execution due to the 'x' flag

More set commands in bash scripting!!

- set -o nounset = set -u option (they are the same, they dont run a script if there is a variable that is uninitialised
-The 'set -o errexit' option is also equivalent to the 'set -e' option because it
#stops the rest of the code from running when there is an error in the code 
-The 'set -o pipefail' option will prevent the grep command from running because
# the file issued is nonexistent

Reading Enviroment variables 

- Reading enviroment variables allows you to restore and retrieve important information within our bash script
- understanding how to work with enviroment variables can greatly enhance scripting capabilities 
- Enviroment variables are like containers with valuable information for our scripts 
- they provide a way to store settings and configurations that our scripts can access when needed  



