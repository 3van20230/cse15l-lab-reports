cd Command:
Example with no arguments:
```
cd
```
input output:
```
[user@sahara ~]$ cd
```
It not an error
Working Directory: Home directiory, changing to the home directory has no output, The command brings you to your home directory.

Example with a path: 
```
cd lecture1
```
input output:
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$
```
It not an error
Working Directory: can write in any directory, changes the working directory to lecture1. 
Example with a path to a file:
```
cd lectuer1/messages/es-mx.txt
```
input output:
```
[user@sahara ~]$ cd lectuer1/messages/es-mx.txt
bash: cd: lectuer1/messages/es-mx.txt: No such file or directory
```
It an error
Working Directory: Any directory. Results in an error because you cannot change the working directory to a file.









ls Command:
Example with no arguments:
```
ls
```
input output:
```
[user@sahara ~]$ ls
lecture1
```
It not an error
Working Directory: Lists the contents of the current directory.
Example with a path:
```
ls lecture1/messages
```
input output:
```
[user@sahara ~]$ ls lecture1/messages
en-us.txt  es-ar.txt  es-mx.txt  zh-cn.txt
```
It not an error
Working Directory:  Lists the contents of the messages directory within the workspace.

Example with a path to a file:
```
ls lecture1/messages/es-ar.txt
```
input output:
```
[user@sahara ~]$ ls lecture1/messages/es-ar.txt
lecture1/messages/es-ar.txt
```
It an error
Working Directory: Results in an error because you cannot list the contents of a file. 



cat Command:
Example with no arguments:
```
cat
```
input output:
```
[user@sahara ~]$ cat
```
It not an error
Working Directory: Waits for input from the user. 
Example with a path
```
cat lecture1/messages
```
input output:
```
[user@sahara ~]$ cat lecture1/messages
cat: lecture1/messages: Is a directory
```
It an error
Working Directory: Results in an error since you cannot concatenate the contents of a directory.


Example with a path to a file
```
cat lecture1/messages/es-ar.txt
```
input output:
```
[user@sahara ~]$ cat lecture1/messages/es-ar.txt
¡Hola Mundo!
```
It not an error
Working Directory: Displays the contents of es-ar.txt located in the messages directory within the workspace.

