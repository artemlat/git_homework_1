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
$ git commit -m 'add new.json
```

### 9. Send the file “new.json” to the external repository:

```




