# #1 GIT Homework  
*Here I learned how to create repositories, synchronize external and internal repositories and push file to them:*
### 4. Create an external repository named "JSON".

*-Go to https://github.com/*  
*-Press [New]*  
*-Input repository name "JSON"*  
*-Press on checkbox "Add a README file"*  
*-Press [Create a repository]* 

### 5. Clone the repository "JSON" to the local computer:

*-Press [Code]*    
*-Copy link git@github.com:artemlat/JSON.git*  
*-Go to the local directory where local repository must be placed*  
*-Open Git Bash*  

```
artem@DESKTOP-4FHC137 MINGW64 /d/github
$ git clone git@github.com:artemlat/JSON.git
Cloning into 'JSON'...
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```

### 6. In the local "JSON" create a file “new.json”:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github
$ cd JSON/

artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ touch new.json
```

### 7. Add the file “new.json” to git:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git add new.json
```

### 8. Commit the file “new.json”:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git commit -m 'add new.json'
[main 681c44d] add new.json
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.json
```

### 9. Send the file “new.json” to the external repository:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 270 bytes | 270.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/JSON.git
   f21de24..681c44d  main -> main
```
   
### 10. Update the content of the file “new.json” - add information about myself (SNM, age, pets quantity, future wish salary) using JSON format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ vim new.json
```
*Press `Enter`*  
*Press `INS`*

```
{
"SNM": "Latyshev Artem Alexandrovich",
"age": 26,
"pets_quantity": 1,
"future_wish_salary": 1000
}
```

*Press `ESC`*

```
:wq
```

*Press `Enter`*

### 11. Send all changes to the external repository:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git commit -am 'updated new.json'
warning: LF will be replaced by CRLF in new.json.
The file will have its original line endings in your working directory
[main f20e461] updated new.json
 1 file changed, 6 insertions(+)

artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 369 bytes | 369.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/JSON.git
   681c44d..f20e461  main -> main
```

### 12. 




