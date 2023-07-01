# #1 GIT Homework  
*Here I learned how to create repositories, synchronize external and internal repositories and push file to them:*

### 4. Create an external repository named "JSON":

*-Go to https://github.com/*  
*-Press `New`*  
*-Input repository name "JSON"*  
*-Press on checkbox "Add a README file"*  
*-Press `Create a repository`* 

### 5. Clone the repository "JSON" to the local computer:

*-Press `Code`*    
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
*-Press `Enter`*  
*-Press `INS`*

```
{
"SNM": "Latyshev Artem Alexandrovich",
"age": 26,
"pets_quantity": 1,
"future_wish_salary": 1000
}
```

*-Press `ESC`*

```
:wq
```

*-Press `Enter`*

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

### 12. Create a file preferences.json:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ touch preferences.json
```

### 13. Add to file "preferences.json" information about my preferences (favourite film, favourite series, favourite food, favourite season, country wanted to visit) using JSON format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ vim preferences.json
```

*-Press `Enter`*  
*-Press `INS`*

```
{
"favourite film": "Marvel films",
"favourite series": "The walking dead",
"favourite food": "meat",
"favourite season": "Spring",
"country wanted to visit": "Norway"
}
```
*-Press `ESC`*

```
:wq
```

*-Press `Enter`*

### 14. Create a file "skills.json", add information about skills that will be learned on the course using JSON format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ cat >> skills.json

artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ cat > skills.json
{
"first skill": "testing theory",
"second skill": "git, bash commands",
"third skill": "Postman",
"fourth skill": "SQL",
"fifth skill": "Devtools"
}
```
### 15. Send 2 files to the external repository:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git add .
warning: LF will be replaced by CRLF in preferences.json.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in skills.json.
The file will have its original line endings in your working directory

artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git commit -m 'add 2 files: skills.json and preferenses.json'
[main a29f452] add 2 files: skills.json and preferenses.json
 2 files changed, 14 insertions(+)
 create mode 100644 preferences.json
 create mode 100644 skills.json

artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 619 bytes | 619.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/JSON.git
   f20e461..a29f452  main -> main
```

### 16. On web interface create a file "bug_report.json":

*-Go to web JSON repository*  
*-Press `Add file`, `Create new file`*  
*-Input name of the file `bug_report.json`*  

### 17. Save changes on web interface:  

*-Press `Commit changes`*

### 18. On web interface change the file "bug_report.json" - add bug report in it using JSON format:

*-Enter a file "bug_report.json" on web interface*  
*-Press `Edit this file`*

```
{
  "id": 1,
  "environment": "Windows 10, Chrome 112",
  "summary": "No icon of the quote in the widget on the main screen",
  "steps": [
    "1. open the app",
    "2. tap on the widget banner",
    "3. tap on [Confirm]",
    "4. collapse the app",
    "5. go to the main screen"
  ],
  "ER": "Quote icon is displayed in the widget",
  "AR": "Quote icon is displayed in the widget",
  "attachments": "link" 
}
```
### 19. Save changes on web interface:

*-Press `Commit changes`*

### 20. Synchronize external and local JSON repository:

*-Go to local JSON repository and open bash console*  

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ git pull
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 1.45 KiB | 14.00 KiB/s, done.
From github.com:artemlat/JSON
   a29f452..c3211d9  main       -> origin/main
Updating a29f452..c3211d9
Fast-forward
 bug_report.json | 16 ++++++++++++++++
 1 file changed, 16 insertions(+)
 create mode 100644 bug_report.json
 ```
 
 ### 21. Create an external repository named "XML":
 
*-Go to https://github.com/*  
*-Press `New`*  
*-Input repository name "XML"*  
*-Press on checkbox "Add a README file"*  
*-Press `Create a repository`* 

### 22. Clone the repository "JSON" to the local computer:

*-Press `Code`*    
*-Copy link git@github.com:artemlat/XML.git*  
*-Go to the local directory where local repository must be placed*  
*-Open Git Bash*

```
artem@DESKTOP-4FHC137 MINGW64 /d/github
$ git clone git@github.com:artemlat/XML.git
Cloning into 'XML'...
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```

### 23. In the local "XML" create a file “new.xml”:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github
$ cd XML/

artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ touch new.xml
```

### 24. Add the file “new.xml” to git:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git add new.xml
```

### 25. Commit the file “new.xml”:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git commit -m 'new.xml add'
[main f108225] new.xml add
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.xml
```

### 26. Send the file “new.xml” to the external repository:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 270 bytes | 270.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/XML.git
   74735d7..f108225  main -> main
```

### 27. Update the content of the file “new.xml” - add information about myself (SNM, age, pets quantity, future wish salary) using XML format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ vim new.xml
```
*-Press `Enter`*  
*-Press `INS`*

```
<info>
    <SNM>Latyshev Artem Alexandrovich</SNM>
    <age>26</age>
    <pets_quantity>1</pets_quantity>
    <future_wish_salary>1000</future_wish_salary>
</info>
```

*-Press `ESC`*

```
:wq
```

*-Press `Enter`*

### 28. Send all changes to the external repository:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git commit -am 'update new.xml'
warning: LF will be replaced by CRLF in new.xml.
The file will have its original line endings in your working directory
[main a30efca] update new.xml
 1 file changed, 6 insertions(+)

artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 385 bytes | 385.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/XML.git
   f108225..a30efca  main -> main

```

### 29. Create a file preferences.xml:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ touch preferences.xml
```

### 30. Add to file "preferences.xml" information about my preferences (favourite film, favourite series, favourite food, favourite season, country wanted to visit) using XML format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ vim preferences.json
```

*-Press `Enter`*  
*-Press `INS`*

```
<preferences>
        <favourite_film>Marvel films</favourite_film>
        <favourite_series>The walking dead</favourite_series>
        <favourite_food>meat</favourite_food>
        <favourit_season>Spring</favourit_season>
        <country_wanted_to_visit>Norway</country_wanted_to_visit>
</preferences>

```

*-Press `ESC`*

```
:wq
```

*-Press `Enter`*

### 31. Create a file "skills.xml", add information about skills that will be learned on the course using XML format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ touch skills.xml

vim skills.xml
```

*-Press `Enter`*  
*-Press `INS`*

```
<skills>
        <first_skill>testing theory</first_skill>
        <second_skill>git, bash commands</second_skill>
        <third_skill>Postman</third_skill>
        <fourth_skill>SQL</fourth_skill>
        <fifth_skill>Devtools</fifth_skill>
</skills>
```

*-Press `ESC`*

```
:wq
```

*-Press `Enter`*

### 32. Create commit in one line:  
*We can't create commit in one line in this case because 2 new files "preferences.xml" and "skills.xml" were not added.*

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git add .
warning: LF will be replaced by CRLF in preferences.xml.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in skills.xml.
The file will have its original line endings in your working directory

artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git commit -m 'commit 2 xml files'
[main 84abfff] commit 2 xml files
 2 files changed, 20 insertions(+)
 create mode 100644 preferences.xml
 create mode 100644 skills.xml
 ```
 ### 33. Send 2 files to the external repository:
 
 ```
 artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 617 bytes | 617.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/XML.git
   a30efca..84abfff  main -> main
```

### 34. On web interface create a file "bug_report.xml":

*-Go to web XML repository*  
*-Press [Add file], [Create new file]*  
*-Input name of the file `bug_report.xml`*

### 35. Save changes on web interface:  

*-Press `Commit changes`*

### 36. On web interface change the file "bug_report.xml" - add bug report in it using XML format:

*-Enter a file "bug_report.xml" on web interface*  
*-Press `Edit this file`*

```
<bug_report>
  <id>1</id>
  <environment>Windows 10, Chrome 112</environment>
  <summary>No icon of the quote in the widget on the main screen</summary>
  <steps>
    <step1>open the app</step1>
    <step2>tap on the widget banner</step2>
    <step3>tap on [Confirm]</step3>
    <step4>collapse the app</step4>
    <step5> go to the main screen</step5>
  </steps>
  <ER>Quote icon is displayed in the widget</ER>
  <AR>Quote icon is displayed in the widget</AR>
  <attachments>link</attachments>
</bug_report>
```

### 37. Save changes on web interface:

*-Press `Commit changes`*

### 38. Synchronize external and local XML repository:

*-Go to local XML repository and open bash console*

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/XML (main)
$ git pull
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 1.48 KiB | 9.00 KiB/s, done.
From github.com:artemlat/XML
   84abfff..4dffa14  main       -> origin/main
Updating 84abfff..4dffa14
Fast-forward
 bug_report.xml | 15 +++++++++++++++
 1 file changed, 15 insertions(+)
 create mode 100644 bug_report.xml
```

### 39. Create an external repository named "TXT":

*-Go to https://github.com/*  
*-Press `New`*  
*-Input repository name "TXT"*  
*-Press on checkbox "Add a README file"*  
*-Press `Create a repository`*

### 40. Clone the repository "TXT" to the local computer:
*-Press `Code`*
*-Copy link git@github.com:artemlat/TXT.git*
*-Go to the local directory where local repository must be placed*
*-Open Git Bash*

```
artem@DESKTOP-4FHC137 MINGW64 /d/github
$ git clone git@github.com:artemlat/TXT.git
Cloning into 'TXT'...
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```

### 41. In the local "TXT" create a file “new.txt”:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github
$ cd TXT/

artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ touch new.txt
```

### 42. Add the file “new.txt” to git:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git add .
```

### 43. Commit the file “new.txt”:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git commit -am 'add file new.txt'
[main 88795f0] add file new.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.txt
```

### 44. Send the file “new.txt” to the external repository:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 272 bytes | 272.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/TXT.git
   ed35a3b..88795f0  main -> main
```

### 45. Update the content of the file “new.txt” - add information about myself (SNM, age, pets quantity, future wish salary) using TXT format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ vim new.txt
```
*-Press `Enter`*  
*-Press `INS`*

```
SNM: Latyshev Artem Alexandrovich,
age: 26,
pets_quantity: 1,
future_wish_salary: 1000
```

*-Press `ESC`*

```
:wq
```

### 46. Send all changes to the external repository:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git commit -am 'update of new.txt'
warning: LF will be replaced by CRLF in new.txt.
The file will have its original line endings in your working directory
[main 9100449] update of new.txt
 1 file changed, 4 insertions(+)

artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 360 bytes | 360.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/TXT.git
   88795f0..9100449  main -> main
```

### 47. Create a file preferences.txt:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ touch preferences.txt
```

### 48. Add to file "preferences.txt" information about my preferences (favourite film, favourite series, favourite food, favourite season, country wanted to visit) using TXT format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/JSON (main)
$ vim preferences.txt
```

*-Press `Enter`*  
*-Press `INS`*

```
{
favourite film: Marvel films,
favourite series: The walking dead,
favourite food: meat,
favourite season: Spring,
country wanted to visit: Norway
}
```
*-Press `ESC`*

```
:wq
```

### 49. Create a file "skills.txt", add information about skills that will be learned on the course using TXT format:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ touch skills.txt

artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ vim skills.txt
```

*-Press `Enter`*  
*-Press `INS`*

```
first skill: testing theory,
second skill: git, bash commands,
third skill: Postman,
fourth skill: SQL,
fifth skill: Devtools
```

*-Press `ESC`*

```
:wq
```

### 50. Create commit in one line:  
*We can't create commit in one line in this case because 2 new files "preferences.txt" and "skills.txt" were not added.*

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git add .
warning: LF will be replaced by CRLF in preferences.txt.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in skills.txt.
The file will have its original line endings in your working directory

artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git commit -am 'add 2 new files'
[main da03be3] add 2 new files
 2 files changed, 10 insertions(+)
 create mode 100644 preferences.txt
 create mode 100644 skills.txt
```

### 51. Send 2 files to the external repository:

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git push
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 541 bytes | 541.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:artemlat/TXT.git
   9100449..da03be3  main -> main
```

### 52. On web interface create a file "bug_report.txt":

*-Go to web TXT repository*  
*-Press `Add file`, `Create new file`*  
*-Input name of the file `bug_report.txt`*

### 53. Save changes on web interface:  

*-Press `Commit changes`*

### 54. On web interface change the file "bug_report.txt" - add bug report in it using TXT format:

*-Enter a file "bug_report.xml" on web interface*  
*-Press `Edit this file`*

```
bug_report
  id: 1
  environment: Windows 10, Chrome 112
  summary: No icon of the quote in the widget on the main screen
  steps:
    step1: open the app
    step2: tap on the widget banner
    step3: tap on [Confirm]
    step4: collapse the app
    step5: go to the main screen
  
  ER: Quote icon is displayed in the widget
  AR: Quote icon is displayed in the widget
  attachments: link
```

### 55. Save changes on web interface:

*-Press `Commit changes`*

### 56. Synchronize external and local XML repository:

*-Go to local XML repository and open bash console*

```
artem@DESKTOP-4FHC137 MINGW64 /d/github/TXT (main)
$ git pull
Enter passphrase for key '/c/Users/artem/.ssh/id_rsa':
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 1.43 KiB | 14.00 KiB/s, done.
From github.com:artemlat/TXT
   da03be3..900fb0f  main       -> origin/main
Updating da03be3..900fb0f
Fast-forward
 bug_report.txt | 14 ++++++++++++++
 1 file changed, 14 insertions(+)
 create mode 100644 bug_report.txt
 ```
 




















 

















 







 
 


















