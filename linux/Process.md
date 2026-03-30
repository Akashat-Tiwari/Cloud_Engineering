## Process :

* One or more related tasks (threads) executing on the computer, not a command or program : a single command can start multiple processes simultaneously

* ps : used to display current running processes

* ps -ef : used to display all the processes in the system in full detail

* pstree : display process in a tree diagram form (relationship b/w process and its parent processes)

PiD : unique Process ID number

TiD : Thread ID number, same as Pid if process is single-threaded. For multi threaded processes , each thread shares the same Pid but has a unique Tid

### Priority of Processes and manipulating the priority :

* To see the priority of the processes use : ps lf 

* priority can be Seen by niceness of a process or priority can be set by niceness : NI , lower the niceness -> higher the priority

* to change the niceness (NI) of a process use : renice +x PID , x = increment in old NI to get the new NI

* you can increase NI but can only decrease the NI by super user or Rootuser ie use sudo before

### foreground Job : a job that runs directly from the shell 

### background job : will be executed at lower priority which in turn will allow smooth execution

* ctrl + c : terminates a foreground process

* ctrl + z : suspend a foreground process

* bg and fg : used to run background and foreground process

### The top command :

* used to interactively monitor the processes (better as compared to repeatedly using ps command)

* refresh itself in 2-3 seconds interval (by default)

## File Operations : 

* creating (also editing) a file without editor : using echo

* echo lineOne > filename : remove older content and insert lineOne (if file not exists then it will create it as well)

* echo lineTwo >> filename : append the content without deleting older one 

## Text Editors : 

* nano : a simple text based editor

* gedit : a simple graphical editor

* vi and emacs : advanced text based editor and graphical editor

### nano : 

* to open a file : nano filename (will create if not exists)

* to save : ctrl + x

* to compile (on main terminal) : gcc filename

* to print output : ./a.out

* to print file : cat filename

### vi (or latest : Vim ie. Vi improved): 

* vi myfile : start the editor and edit myfile

* :r file2 : read in file2 and insert at current position

* :w : write to file2

* :w myfile: write out to myfile

* :w! file2 : overwrite file2

* :x : exit

* :q : quit

* :q! : quit even though modifications have not been saved

* {important} :wq : exit vi and save the file

### modes in vi : 

* by default :  command mode

* type i to enter insert mode (used to insert content) and esc to return back to command mode

* type : to enter line mode (each key is an external command) and esc to return back to command mode
