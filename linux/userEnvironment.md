### About user : 

* whoami :  identify the current user

* who : list the currently logged on users

* su : substitute user or switch user -> normal user to root user

* sudo : superUser Do Or rootuser Do -> let a normal user run a command with administrator (root) privilages

### Environment Variables : 

* are quantities that have specific values which maybe utilised by the CLI such as bash

### shortcuts : 

* ctrl + L : clears the screen

* ctrl + D : exits the current shell 

* ctrl + Z : suspend the current process

* ctrl + C : cancel/kill the current process
 
* ctrl + H : works the same as backspace

* ctrl + A : goes to the beginning of the line

* ctrl + W : deletes the word before the cursor
 
* ctrl + U : deletes from the beginning of line to the cursor position

* ctrl + E : goes to the end of the line

### Manipulating Text :

* cat fileName : often used to read and print file (simply means viewing file contents)

* cat file1 file2 : used to concatenate multiple files and display the output (content of first followed by second)

* cat file1 file2 > file3 : concatenate multiple files and send it to new file3


* tac filename : display the file in reverse order means line is exactly same but the order is reversed (ending line to starting line)

* tac file1 file2 : first file then second but reverse order

* less file1 or cat file1 | less : opening a large file directly in editor will cause issues due to high memory utilization, instead , use less file1 to open file page by page without entire file in memory before starting

* sed and awk is used to manipulate data files

### file manipulation utilities :

* sort file1 : sort the lines in the specified file, according to the characters at the beginning of each line

* uniq : used to remove duplicate consecutive lines (often used with sort as consecutive lines are required) only prints the file after operation not actually edit it (sort -u filename or sort filename | uniq) 
 
* paste :

* join :

* split :

### Network Operations : 

* 




