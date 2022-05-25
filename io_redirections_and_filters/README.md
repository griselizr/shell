<h1> 🐚 Shell, I/O Redirections and filters 🏹 </h1>
<h2> Learning Objectives 🎯 </h2>

Shell, I/O Redirection

    What do the commands head, tail, find, wc, sort, uniq, grep, tr do
    How to redirect standard output to a file
    How to get standard input from a file instead of the keyboard
    How to send the output from one program to the input of another program
    How to combine commands and filters with redirections

Special Characters

    What are special characters
    Understand what do the white spaces, single quotes, double quotes, backslash, comment, pipe, command separator, tilde and how and when to use them

Other Man Pages

    How to display a line of text
    How to concatenate files and print on the standard output
    How to reverse a string
    How to remove sections from each line of files
    What is the /etc/passwd file and what is its format
    What is the /etc/shadow file and what is its format

Requirements
General

    Allowed editors: vi, vim, emacs
    All your scripts will be tested on Ubuntu 20.04 LTS
    All your scripts should be exactly two lines long ($ wc -l file should print 2)
    All your files should end with a new line (why?)
    The first line of all your files should be exactly #!/bin/bash
    A README.md file, at the root of the folder of the project, describing what each script is doing
    You are not allowed to use backticks, &&, || or ;
    All your files must be executable
    You are not allowed to use sed or awk

More Info

Read your /etc/passwd and /etc/shadow files.

Note: You do not have to learn about fmt, pr, du, gzip, tar, lpr, sed and awk yet.
<h2> TASKS </h2>
   
   <strong> 0. Hello World </strong>
    <p> Write a script that prints “Hello, World”, followed by a new line to the standard output. </p>

   <strong> 1. Confused smiley </strong> 
    <p> Write a script that displays a confused smiley "(Ôo)'.</p>
    <strong> 2. Let's display a file </strong> 
   <p> Display the content of the /etc/passwd file.</p>
   <strong>  3. What about 2?</strong> 
   <p> Display the content of /etc/passwd and /etc/hosts </p>
   <strong>  4.  Last lines of a file </strong> 
   <p> Display the last 10 lines of /etc/passwd</p>
   <strong>  5.I'd prefer the first ones actually </strong> 
  <p> Display the first 10 lines of /etc/passwd</p>
    <strong> 6. Line #2 </strong> 
   <p> Write a script that displays the third line of the file iacta.</p>
   The file iacta will be in the working directory </p>
    <li> You’re not allowed to use sed </li>
    <strong> 7. It is a good file that cuts iron without making a noise </strong> 
    <p> Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line. </p>
    <strong> 8. Save current state of directory </strong> 
   <p> Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it. </p>
  <strong>   9.Duplicate last line </strong> 
   <p> Write a script that duplicates the last line of the file iacta </p>

  <li>  The file iacta will be in the working directory</li>
   <strong>  10. No more javascript  </strong> 
   <p>Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.</p>
   <strong>  11. Don't just count your directories, make your directories count </strong> 
   <p> Write a script that counts the number of directories and sub-directories in the current directory.</p>
   <li> The current and parent directories should not be taken into account </li>
    <li>Hidden directories should be counted</li>
   <strong>  12. What’s new </strong> 
   <p> Create a script that displays the 10 newest files in the current directory.
    Requirements:</p>
   <li> One file per line</li>
    <li>Sorted from the newest to the oldest </li>
   <strong>  13.Being unique is better than being perfect </strong> 
    <p>Create a script that takes a list of words as input and prints only words that appear exactly once. </p>
    <li>Input format: One line, one word</li>
    <li>Output format: One line, one word</li>
    <li>Words should be sorted</li>
   <strong> 14.It must be in that file  </strong> 
    <p>Display lines containing the pattern “root” from the file /etc/passwd</p>
   <strong>  15.Count that word  </strong> 
    <p>Display the number of lines that contain the pattern “bin” in the file /etc/passwd</p>
    <strong> 16.What's next?  </strong> 
   <p> Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.</p>
   <strong>17.I hate bins</strong>
   <p> Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.</p>
   <strong> 18.Letters only please </strong>
   <p>Display all lines of the file /etc/ssh/sshd_config starting with a letter.</p>
     <li>include capital letters as well</li>
     <strong>19.A to Z </strong>
    <p>Replace all characters A and c from input to Z and e respectively.</p>
    <strong> 20.Without C, you would live in hiago</strong>
    <p> Create a script that removes all letters c and C from input.</p>
    <strong>21.esreveR </strong>
    <p> Write a script that reverse its input.</p>
    <strong>22.DJ Cut Killer  </strong>
    <p> Write a script that displays all users and their home directories, sorted by users.</p>
   <li> Based on the the /etc/passwd file</li>
   <strong> 23.Empty casks make the most noise </strong>
   <p> Write a command that finds all empty files and directories in the current directory and all sub-directories.</p>
   <li> Only the names of the files and directories should be displayed (not the entire path)</li>
   <li> Hidden files should be listed </li>
   <li>One file name per line</li>
   <li> The listing should end with a new line </li>
   <li> You are not allowed to use basename, grep, egrep, fgrep or rgrep </li>
   <strong> 24.A gif is worth ten thousand words </strong>
   <p> Write a script that lists all the files with a .gif extension in the current directory and all its sub-directories.</p>
   <li>Hidden files should be listed</li>
   <li>Only regular files (not directories) should be listed</li>
   <li>The names of the files should be displayed without their extensions</li>
   <li>The files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay) </li>
   <li>One file name per line</li>
   <li>The listing should end with a new line</li>
   <li>You are not allowed to use basename, grep, egrep, fgrep or rgrep</li>
   <strong>25.Acrostic </strong>
   <p>An acrostic is a poem (or other form of writing) in which the first letter (or syllable, or word) of each line (or paragraph, or other recurring feature in the text) spells out a word, message or the alphabet. The word comes from the French acrostiche from post-classical Latin acrostichis). As a form of constrained writing, an acrostic can be used as a mnemonic device to aid memory retrieval</p>
   <p>Create a script that decodes acrostics that use the first letter of each line.</p>
    <li>The ‘decoded’ message has to end with a new line</li>
    <li>You are not allowed to use grep, egrep, fgrep or rgrep</li>
    <strong>26.The biggest fan </strong>
   <p>Write a script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.</p>
   <li>Order by number of requests, most active host or IP at the top</li>
   <li>You are not allowed to use grep, egrep, fgrep or rgrep </li>
   
