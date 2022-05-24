<h1> Shell, permissions </h1>


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
    Create a script that switches the current user to the user betty.
     <li>You should use exactly 8 characters for your command (+1 character for the new line)</li>
     <li>You can assume that the user betty will exist when we will run your script</li>

    <strong> 1. Who am I </strong> 
    Write a script that prints the effective username of the current user.
    <strong> 2. Groups</strong> 
    Write a script that prints all the groups the current user is part of.
   <strong>  3. New Owner</strong> 
    Write a script that changes the owner of the file hello to the user betty.
   <strong>  4. Empty!</strong> 
    Write a script that creates an empty file called hello.
   <strong>  5. Execute </strong> 
    Write a script that adds execute permission to the owner of the file hello.
    <strong> 6. Multiples Permissions</strong> 
    Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
    The file hello will be in the working directory
    <strong> 7. Everybody!</strong> 
    Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello
    <li>The file hello will be in the working directory </li>
    <li>You are not allowed to use commas for this script</li>
    <strong> 8. James Bond</strong> 
    Write a script that sets the permission to the file hello as follows:

    Owner: no permission at all
    Group: no permission at all
   <li> Other users: all the permissions </li>
    <li>The file hello will be in the working directory You are not allowed to use commas for this script</li>
  <strong>   9. John Doe</strong> 
    Write a script that sets the mode of the file hello to this:
    -rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
   <strong>  10. Look in the mirror </strong> 
    Write a script that sets the mode of the file hello the same as olleh’s mode.
<li>The file hello will be in the working directory </li>
<li>The file olleh will be in the working directory </li>
   <strong>  11. Directories</strong> 
    Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.     Regular files should not be changed.
   <strong>  12. More Directories</strong> 
    Create a script that creates a directory called my_dir with permissions 751 in the working directory.
   <strong>  13. Change Group </strong> 
    Write a script that changes the group owner to school for the file hello
    <li>The file hello will be in the working directory </li>
   <strong>  14. Owner & Group </strong> 
    Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
   <strong>  15. Symbolics links </strong> 
    Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.

    <li>The file _hello is in the working directory </li>
    <li>The file _hello is a symbolic link </li>
    <strong> 16. If only </strong> 
    Write a script that changes the owner of the file hello to vincent only if it is owned by the user guillaume.
   <li> The file hello will be in the working directory </li>

