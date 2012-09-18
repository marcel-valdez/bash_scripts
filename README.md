To add these files to your bash environment, add this line to the end of your $HOME/.bashrc file:
````bash
PATH = $PATH:$HOME/bash_scripts
````
Asuming you added the bash_scripts folder in $HOME/bash_scripts.

git_pull_all will pull git repositories in four MPI connected machines with hostnames: proc0, proc1 ... proc3
example:
````bash
user@host:~$ git_pull_ull
````

git_push will push the current repository to the remote origin
example:
````bash
user@host:~$ git_push "Commit message"
````

git_push_pull will execute git_push then git_pull_all
example:
````bash
user@host:~$ git_push_pull "Commit message"
````

make_errors will execute make and filter all messages to only show error messages, and filter out warnings and verbose stuff.
example:
````bash
user@host:~$ make_errors all
````

make_warnings will execute make and print only Warnings and Errors from make
example:
````bash
user@host:~$ make_warnings all
````

para_exec will execute any commando in four MPI connected machines with hostnames: proc0, proc1 ... proc3
example:
````bash
user@hprocX:~$ hostname
proc0
proc1
proc2
proc3
````



