# up

### Purpose

up is a simple utility used during the active development of a remote project. 
It allows the user to work on projects on their local system, and upload the modified files to a remote working directory.

### Usage

Use `up init` on a directory that you want to use as a local working directory.
You will be prompted to enter a base (either an alias or a hostname), and a destination (the filepath on remote directory where the files will be stored).

Subsequently, use the `up` command to 'push' changes to the working directory to the remote destination. The command will handle addition of new files, modification of existing files, and deletion of files.

Use `up reset` to remove all traces of the utility on a working directory.
Use `up force` to force all files in the directory to be re-uploaded.

### Remarks

This utility was born out of a terribly laggy internet connection to my remote system. There was a project that could only be effectively tested on the remote system, but using vim on a ssh session proved to infeasible. I decided to work on the files locally, and scp them as needed. I thought that automating this process would be fun, and could come in handy in the future. I took the chance to improve my familiarity with bash as well. 
