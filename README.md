# Bash-Scripting
Project 02 for Object-Oriented Programming

This is a tutorial using a reference: https://linuxconfig.org/bash-scripting-tutorial-for-beginners


I am going to list chronologically the steps I've taken for this lab: 

(Lines with -- note a problem that needs fixing)

-Created task.sh using "nano task.sh" then added these cmds "date, pwd, ls" Note: "cal" was not available.
-Ran task.sh using "chmod +x task.sh"
-Used "which bash" to locate bash directory
-Added "#!/usr/bin/bash" to file task.sh
-Created file date.sh using "echo date > date.sh" this cmd created date.sh and added cmd "date" within the file.
-You can use "bash date.sh" to also run a script without making it an executable.
-Created hello-world.sh echoing "Hello World".

--Created backup.sh and had trouble with the "tar -czf" cmd. Couldn't find a working directory to create the backup(tried many different directories).

-Created welcome.sh using cmds given(I thought this was badass)

--Updated backup.sh and this was the error given:
"tar: /home/razor: Cannot stat: No such file or directory
tar: Exiting with failure status due to previous errors
Backup of /home/razor completed! Details about the output backup file:
rw-r--r-- 1 razor 197609 45 Oct  4 19:17 /tmp/razor_home_2020-10-04_191757.tar.gz"
NOTE: It only says it was completed because of the "echo" cmd.

-Updated backup.sh to remove the unwanted stderr.

--Still having issues with directory path in backup.sh but updated the file to contain the functions/code given in tutorial.

-Created comparison.sh and used the code given. This shows whether 2 distinct scripts are different. With 1 being TRUE and 0 being FALSE.
-Created if_else.sh and updated it with code given.
-Updated backup.sh to include if_else statements. This shows the number of files updated before and after the backup.
-Updated the backup.sh to let the user decide which directory will be backed up. Default is home directory(Home directory is not found)
-Created bash-loops.sh as an example of how bash loops work.
-Created while-loops.sh. Does the same thing as bash loops but shows a different approach.
-Created until-loops.sh. Does the exact opposite as a while loop.
(NOTE: I created these files to show the examples for myself.)

--The backup.sh script is not displaying any output when I added the Until loops code. So, i created a seperate backup script known as backup2 that contains that code until I figure out the problem.
IMPORTANT: The backup.sh is not updated with the until loops. It is the same as it was under the positional parameters section.

*I feel like the loop at lines 59-61 in backup2.sh are causing the issue. Because a working directory is still not found.

Sources:
Rendek, Lubos. “Bash Scripting Tutorial for Beginners.” Linux Tutorials - Learn Linux Configuration, 27 May 2020, linuxconfig.org/bash-scripting-tutorial-for-beginners. 

“First Steps with Git: Clone, Add, Commit, Push.” Earth Data Science - Earth Lab, 12 Sept. 2017, www.earthdatascience.org/workshops/intro-version-control-git/basic-git-commands/. 









