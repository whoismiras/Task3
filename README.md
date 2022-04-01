# Task3
### Miras Ramazanov 
### Git Testing Tasks



## Task 1:
<br>•	Stage all new, modified, and deleted files. Use the shorthand command:
git add –A
<br>•	Show the possible options for the status command in command line:         git status –help
<br>•	Create, and move to a new branch with the name hello-you:     	         git checkout –b hello-you
<br>•	Get all the change history of the origin for this branch: git fetch origin
<br>•	In .gitignore add a line to ignore all .temp files: *.temp
<br>•	Replace the remote URL for origin with x/y.git on abc.com using SSH:           git remote set-url origin git@abc.com:x/y.git  



## Task 2: 
#### 1) Fork & Pull Request
<br>git clone https://github.com/whoismiras/forking_exercise.git
<br>git branch Develop
<br>git checkout Develop
<br>nano 1.txt “File Created”
<br>git status
<br>git add 1.txt
<br>git commit –m “1st file”
<br>git push –set-upstream origin Develop
#### 2) Change to a different branch and add some files and merge into main when you are done.
<br>git branch second
<br>git checkout second
<br>git branch
<br>nano File1.txt
<br>nano File2.txt
<br>git add .
<br>git status
<br>git commit –m “created 2 files”
<br>git checkout main
<br>git merge second
#### 3) Submit another pull request, with squashed commits.
<br>git checkout Develop
<br>git log
<br>git rebase –i HEAD1
<br>git checkout
<br>git checkout second
<br>nano File3.txt
<br>nano File4.txt
<br>git add .
<br>git commit –m “file 3-4”
<br>git rebase –i HEAD2
<br>git push –set-upstream origin second



## Task 3:
#### 1) Сгенерируйте конфликт на main. Напишите решение
<br>cd IdeaProjects/
<br>mkdir Task3
<br>cd Task3/
<br>git clone https://github.com/whoismiras/Task3.git
<br>nano 1.txt
<br>git add 1.txt
<br>git commit –m “1st file”
<br>git push 
<br>Создаем (имитируем) изменения файла на github.com
<br>nano 1.txt
<br>git add .
<br>git commit –m “2nd file”
<br>git pull
<br>nano 1.txt
<br>git add .
<br>git commit “3”
<br>git push
#### 2) Потом сгенерируйте конфликт в бранче. Тоже напишите решение.
<br>git branch Develop
<br>nano 1.txt
<br>git merge main
<br>nano 1.txt
<br>git add .
<br>git commit –m “solved conflict”
<br>git push



## Task 4:
#### 1)	Cоздать 2 файла, разделить их на 2 push
<br><br>nano 2.txt
<br>nano 3.txt
<br>git add 2.txt
<br>git stash
<br>git commit –m “first push”
<br>git push
<br>git stash pop
<br>git add 3.txt
<br>git stash
<br>git commit -m "second push"
<br>git push 



## Task 5:
#### 1)	Add 5 blocks of information into text, commit and push only 3 of them, without deleting any content.
<br>nano 5.txt
<br>git add –p 5.txt
<br>git commit –m “blocks”
<br>git push



