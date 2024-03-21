# Linux-40-command-
**1 .File and Folder Permission CHOWN, CHMOD, CHGRP)**

**CHMOD**

This command is used to change the permissions of a file or directory. It stands for "change mode." The permissions can be modified for three categories of users: the owner of the file or directory, the group associated with the file or directory, and others.

Here's a breakdown of the permissions:

Read (r): Users can read the contents of the file or directory.
Write (w): Users can modify the contents of the file or directory.
Execute (x): For files, it allows users to execute the file if it's a program or script. For directories, it allows users to enter and access files within the directory.
Permissions are represented by three sets of characters: one for the owner, one for the group, and one for others. For example: chmod u+x file.txt grants the owner of file.txt the permission to execute it.
```
ls -l file.txt
```

```
chmod u+x,g-w,o-rx file.txt
```

**Output**

![Screenshot from 2024-03-21 14-35-07](https://github.com/MOINUDDIN0786/Linux-40-command-/assets/64195957/44a59aed-dead-4b3c-beb8-6e325e6b8742)


**CHOWN**

This command is used to change the ownership of a file or directory. It stands for "change owner." You can specify both the user and group ownership of the file or directory. For example: chown user:group file.txt changes the ownership of file.txt to the user and group specified.

```
chown user2:group2 file.txt
```
```
ls -l file.txt
```
**Output**

-rwxr----- 1 user2 group2 0 Mar 21 12:00 file.txt

**CHGRP**

This command is used to change the group ownership of a file or directory. It stands for "change group." Unlike chown, it only modifies the group ownership. For example: chgrp group file.txt changes the group ownership of file.txt to the specified group.


```
chgrp group3 file.txt
```
```
 ls -l file.txt
```
**Output**

-rwxr----- 1 user2 group3 0 Mar 21 12:00 file.txt

**2 .Check File/Folder/Content (LS, LL, CAT, GREP, HEAD, TAIL, LESS, MORE, ECHO)**

**LS**

Ls is used to all list inside directory.

```
ls folderName
```




