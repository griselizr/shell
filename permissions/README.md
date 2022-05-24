<h1> Shell, permissions </h1>  :shell: :page_with_curl:


Permissions

    What do the commands chmod, sudo, su, chown, chgrp do
    Linux file permissions
    How to represent each of the three sets of permissions (owner, group, and other) as a single digit
    How to change permissions, owner and group of a file
    Why can’t a normal user chown a file
    How to run a command with root privileges
    How to change user ID or become superuser

Other Man Pages

    How to create a user
    How to create a group
    How to print real and effective user and group IDs
    How to print the groups a user is in
    How to print the effective userid

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
<h2> TASKS </h2>
   
   <strong> 0. My name is Betty </strong>
    <p> Create a script that switches the current user to the user betty. </p>
     <li>You should use exactly 8 characters for your command (+1 character for the new line)</li>
     <li>You can assume that the user betty will exist when we will run your script</li>

   <strong> 1. Who am I </strong> 
    <p>Write a script that prints the effective username of the current user.</p>
    <strong> 2. Groups</strong> 
   <p> Write a script that prints all the groups the current user is part of.</p>
   <strong>  3. New Owner</strong> 
   <p> Write a script that changes the owner of the file hello to the user betty.</p>
   <strong>  4. Empty!</strong> 
   <p> Write a script that creates an empty file called hello.</p>
   <strong>  5. Execute </strong> 
  <p> Write a script that adds execute permission to the owner of the file hello.</p>
    <strong> 6. Multiples Permissions</strong> 
   <p> Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
    The file hello will be in the working directory </p>
    <strong> 7. Everybody!</strong> 
    <p>Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello. </p>
    <li>The file hello will be in the working directory </li>
    <li>You are not allowed to use commas for this script</li>
    <strong> 8. James Bond</strong> 
   <p> Write a script that sets the permission to the file hello as follows:
   Owner: no permission at all
    Group: no permission at all </p>
   <li> Other users: all the permissions </li>
    <li>The file hello will be in the working directory You are not allowed to use commas for this script</li>
  <strong>   9. John Doe</strong> 
   <p> Write a script that sets the mode of the file hello to this:
    -rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello </p>
   <strong>  10. Look in the mirror </strong> 
   <p> Write a script that sets the mode of the file hello the same as olleh’s mode.</p>
<li>The file hello will be in the working directory </li>
<li>The file olleh will be in the working directory </li>
   <strong>  11. Directories</strong> 
   <p> Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.      Regular files should not be changed.</p>
   <strong>  12. More Directories</strong> 
   <p> Create a script that creates a directory called my_dir with permissions 751 in the working directory.</p>
   <strong>  13. Change Group </strong> 
    <p>Write a script that changes the group owner to school for the file hello </p>
    <li>The file hello will be in the working directory </li>
   <strong>  14. Owner & Group </strong> 
    <p>Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.</p>
   <strong>  15. Symbolics links </strong> 
    <p>Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.</p>

   <li>The file _hello is in the working directory </li>
    <li>The file _hello is a symbolic link </li>
    <strong> 16. If only </strong> 
   <p> Write a script that changes the owner of the file hello to vincent only if it is owned by the user guillaume.</p>
   <li> The file hello will be in the working directory </li>

