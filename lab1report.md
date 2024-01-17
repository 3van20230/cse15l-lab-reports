cd Command:
Example with no arguments:
```
cd
```
input output:
```
[user@sahara ~]$ cd
```
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
Working Directory: Any directory. Results in an error because you cannot change the working directory to a file.









ls Command:
Example with no arguments:
```
ls
```
Example with a path:
```
ls lectuer1/messages
```
Example with a path to a file:
```
ls lecture1/messages/es-ar.txt
```



cat Command:
Example with no arguments:
```
cat
```

Example with a path
```
cat lectuer1/messages
```

Example with a path to a file
```
cat lectuer1/messages/es-ar.txt
```
I am talking about `cat`
