1. signup to github
2. create repo
3. clone the repo
4. create github token
5. git add . ; git commit -m "some-msg"; git push origin main


Shell Script
---------------
1st line -->#!/bin/bash

shebang is the location interpreter, commands written inside shell script is interpreted and executed by this shebang

zshell
kshell
cshell
fish

bash shell == shell

how to execute shell script
---------------------
sh <script>
bash <script>
./<script-name> --> this should have execute permission
X --> running the command/script

1. repeated words
2. if you want to change, you have to change it every where
3. while changing accidently you may change actual code

variables
------------
int i=0, j=0

i and j are variables

x=0, y=1

derive the formula, submit variables at last

variables hold some values,

4. if you change variable value, it will be automaticaly reflected everywhere it is referred


arguments/parameters
--------------------
sh variables.sh Raheem Robert

Raheem = 1st variable
Robert = 2nd variable
.
.
.
John = nth variable

confidential information
-----------------------
We want user to enter manually before execution

Data types
------------------
integer
float
decimal
string
boolean --> true/false ... 1=true, 0=false
array
arraylist
set, map

array --> list of values
if you define a variable as array, it can hold list of values...

$VARIBALE
${VARIBALE}

+, -, *, / , %

conditions
---------------
when you want to take a decission

I want to check whether a number is greater than 20 or not

first get the number
check if it is greater than 10 or not
if greater print greater
if lesser print lower

if(expression){
	this statement will execute if expression is true
}
else{
	this statement will execute if expression is false
}

NUMBER=5
if(!NUMBER>10){
	print "print given number is greater than 10"
}
else{
	print "print given number is less than 10"
}

NUMBER>10=false, !=false
false false is true

installation
---------------
if you want to install you should have super user access
so check user
if super user, proceed
if not super user, I should throw proper error

How you run a command inside shell script and take the output

if id is 0 then super user, if not 0 then normal user

if error comes, can we proceed? NO

disadvantage of shell script
------------------------
shell script will not stop even it faces the error, it is user responsibility to check the previous command is success/not

exit status
------------
what is exit status?

$? --> to check the exit status of previous command
0 --> success
other than 0 --> failure
1-127

dnf installation commands are 20..

140 lines of validation