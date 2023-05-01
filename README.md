Download Link: https://assignmentchef.com/product/solved-cecs326-homework-1
<br>
Gantt Charts, Linux systems

<ol>

 <li>A) Purpose: This portion of the assignment familiarizes you with the Linux systems at CSULB and gives you practice with shell scripts.</li>

</ol>

General warning: you must run this on the linux server linux1.cecs.csulb.edu. Use the ssh (secure shell) command to reach it. If you are working at home, ssh to 134.139.248.2 with port 2022.

There are three parts.

The purpose of the first part is to get some information (your magic numbers) that you need for the paper (Gantt chart) assignment on resource sharing.

The second part has you build and run a shell script that is almost the same as one from lecture. You may find the code from the lectures in the /net/326/ directory (they start with chap01 in their names).

The third part has you design and build a shell script of your own.

<ul>

 <li>Run the program /net/getmagicnumber. This program delivers you 4 magic numbers that you will need for part B of this homework.</li>

 <li>Build a shell script from lecture. The name of your script file should be called listdirs. It should start with the foreach example from lecture that lists the lib, bin, and src Since you do not have any such diretories, you will need to modify the script so that the first thing it does is change to the /usr directory (use the cd command). This directory does have the needed three subdirectories.</li>

 <li>Build a shell script. The name of your script file should be called getpids.</li>

</ul>

First, the shell script should get your login name (whoami) It should both save your name into a variable and print the contents of that variable (echo) it to the screen.

Second, the script should list all processes (ps aux), use grep -v to eliminate those processes that have your login name in them, then it should only output the pids of those processes (using cut with the column arguments from lecture).

<ol>

 <li>B) Purpose: This portion of the assignment familiarizes you with Gantt charts and process sharing.</li>

</ol>

This assignment uses your 4 magic numbers, that means your answer will be different from any one else. Make sure you write your magic numbers at the top of the homework you submit.

To simplify this there are only two things that a process can do, process and wait. Two processes cannot process at the same time so you will need some delays. (IE, assume this is a single core/thread system)

If some of your magic numbers are 0, it’s your lucky day because it’s very easy to do something that takes 0 time; just don’t processs or wait.

There are three processes:

Process 1: processes 3, waits 4, processes 5;

Process 2: processes 2, waits 2, processes 2, waits 3, processes 1;

Process 3: waits (use magic number 1), processes (use magic number 2), waits (use magic number 3), processes (use magic number 4).


