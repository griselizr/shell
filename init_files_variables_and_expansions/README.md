<h1> 📁Shell, init files, variables and expansions ↔️</h1>
Learning Objectives

At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
General

    What happens when you type $ ls -l *.txt

Shell Initialization Files

    What are the /etc/profile file and the /etc/profile.d directory
    What is the ~/.bashrc file

Variables

    What is the difference between a local and a global variable
    What is a reserved variable
    How to create, update and delete shell variables
    What are the roles of the following reserved variables: HOME, PATH, PS1
    What are special parameters
    What is the special parameter $??

Expansions

    What is expansion and how to use them
    What is the difference between single and double quotes and how to use them properly
    How to do command substitution with $() and backticks

Shell Arithmetic

    How to perform arithmetic operations with the shell

The alias Command

    How to create an alias
    How to list aliases
    How to temporarily disable an alias

Other help pages

    How to execute commands from a file in the current shell

Requirements
General

    Allowed editors: vi, vim, emacs
    All your scripts will be tested on Ubuntu 20.04 LTS
    All your scripts should be exactly two lines long ($ wc -l file should print 2)
    All your files should end with a new line (why?)
    The first line of all your files should be exactly #!/bin/bash
    A README.md file, at the root of the folder of the project, describing what each script is doing
    You are not allowed to use &&, || or ;
    You are not allowed to use bc, sed or awk
    All your files must be executable

Note: You do not have to learn about awk, tar, bzip2, date, scp, ulimit, umask, or shell scripting, yet.
    <strong> 0. <o> </strong>
    <p> Create a script that creates an alias. </p>
    <li> Name: ls</li>
    <li> Value: rm *</li>
    <strong> 1. Hello you </strong>
    <p> Create a script that prints hello user, where user is the current Linux user.</p>
    <strong> 2. The path to success is to take massive, determined action </strong>
    <p> Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.</p>
    <strong> 3. If the path be beautiful, let us not ask where it leads </strong>
    <p>Create a script that counts the number of directories in the PATH.</p>
    <strong> 4. Global variables </strong>
    <p> Create a script that lists environment variables. </p>
    <strong> 5. Local variables </strong>
    <p> Create a script that lists all local variables and environment variables, and functions. </p>
    <strong> 6. Local variable  </strong>
    <p> Create a script that creates a new local variable. </p>
    <strong>  7. Global variable <strong>
    <p> Create a script that creates a new global variable. </p>
        <li> Name: BEST</li>
        <li> Value: School </li>
        <strong> 8. Every addition to true knowledge is an addition to human power </strong>
        <p> Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line. </p>
        <strong> 9. Divide and rule  </strong>
        <p> Write a script that prints the result of POWER divided by DIVIDE, followed by a new line. </p>
        <li> POWER and DIVIDE are environment variables</li>
        <strong> 10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath </strong>
        <p> Write a script that displays the result of BREATH to the power LOVE</p>
        <li> BREATH and LOVE are environment variables</li>
        <li> The script should display the result, followed by a new line </li>
        <strong> 11. There are 10 types of people in the world -- Those who understand binary, and those who don't </strong>
        <p> Write a script that converts a number from base 2 to base 10. </p>
        <li> The number in base 2 is stored in the environment variable BINARY <li>
        <li> The script should display the number in base 10, followed by a new line </li>
        <strong> 12. Combination </strong>
        <p> Create a script that prints all possible combinations of two letters, except oo.</p>
        <li> Letters are lower cases, from a to z </li>
        <li> One combination per line </li>
        <li> The output should be alpha ordered, starting with aa</li>
        <li> Do not print oo </li>
        <li> Your script file should contain maximum 64 characters</li> 
        <strong> 13. Floats </strong>
        <p> Write a script that prints a number with two decimal places, followed by a new line.The number will be stored in the environment variable NUM. </p>
        <strong> 14. Decimal to Hexadecimal </strong>
        <p> Write a script that converts a number from base 10 to base 16. </p>
        <li> The number in base 10 is stored in the environment variable DECIMAL </li>
        <li> The script should display the number in base 16, followed by a new line</li>
        <strong> 15. Everyone is a proponent of strong encryption </strong>
        <p> Write a script that encodes and decodes text using the rot13 encryption. Assume ASCII.</p>
        <strong> 16. The eggs of the brood need to be an odd number </strong>
        <p> Write a script that prints every other line from the input, starting with the first line.</p>
        <strong> 17. I'm an instant star. Just add water and stir. </strong>
        <p> Write a shell script that adds the two numbers stored in the environment variables WATER and STIR and prints the result. </p>
        <li> WATER is in base water </li>
        <li> STIR is in base stir.</li>
        <li> The result should be in base bestchol </li>
