# Introduction to shell scripting
- A shell scripting is a text file that contains a sequence of commands for a unix based operating system

* It is called scripts because it combines a sequence of commands- that would otherwise have to be typed into a keyboard one at a time - into a single script.

* The simple reason why does shell script exists because - we don't want to repeat tasks manually instead we combine all the commands under one umbrella and execute it. 

* The main purpose behind doing this is avoid manual work which was slow and start automating to save time and energy.

# The core problem Shell sscripts is solving...

-Question- “How do I make the computer do a sequence of tasks automatically, reliably, and repeatedly?”

-Ans - Shell scripting = writing a file that contains a sequence of commands + logic to automate tasks.

- Shell is a program that takes your commands and gives them to the operating system to execute.

# A simple workflow of shell 

- You → Shell → Kernel → Hardware

You → give command

Shell → interprets

Kernel → actually does the work

Hardware → executes


# Why shell exists?

- Without shell:

You cannot control system easily

You must write low-level code every time

# Shell gives:

Simplicity

Speed

Automation capability


# Commands are not magic — they are just programs stored in the system.

- instead of typing this every time- 

"cd /var/log

ls

echo "Done" 

You put it inside a file:

cd /var/log

ls

echo "Done"

Save it as: 

myscript.sh

Now instead of 3 commands…

👉 You run 1 file

💥 Automation begins

First Principle Insight

A script is nothing special.

❗ It is just a text file with commands inside it

Same as:

.txt
.log

But:
👉 Shell interprets it as instructions

# What is Shebang (#!)

#!/bin/bash 

What does this mean?

#! → signal to system: “this is a script”

/bin/bash → path to interpreter

So you're saying:

“Run this file using the bash shell”

# Execution flow

When you run a script: ./myscript.sh

System does:

Reads #!

Finds /bin/bash

Passes your script to bash

Bash executes line by line

# Variable in shell scripting

What if data changes?

Example:

Username changes

File name changes

Path changes

👉 You don’t want to rewrite the script every time

💡 Solution

Store data in a container and reuse it

That container = Variable

- for example 

instead of writing 

echo "hello ravindra"

- We say 

name="ravindra"

echo "Hello $name"

# what does it mean

- name → variable

"Ravindra" → value

$name → access value

# what are conditions 

- definition :

"A condition is a test that returns true or false"

example:

-  IF something is true → do this  

-  ELSE → do something else

# Important Operators
🔹 Numbers
-eq → equal

-ne → not equal

-gt → greater than

-lt → less than