# Task3
Miras Ramazanov 
Git Testing Tasks



Task 1:
•	Stage all new, modified, and deleted files. Use the shorthand command:
git add –A
•	Show the possible options for the status command in command line:         git status –help
•	Create, and move to a new branch with the name hello-you:     	         git checkout –b hello-you
•	Get all the change history of the origin for this branch: git fetch origin
•	In .gitignore add a line to ignore all .temp files: *.temp
•	Replace the remote URL for origin with x/y.git on abc.com using SSH:           git remote set-url origin git@abc.com:x/y.git  



Task 2: 
1) Fork & Pull Request
git clone https://github.com/whoismiras/forking_exercise.git
git branch Develop
git checkout Develop
nano 1.txt “File Created”
git status
git add 1.txt
git commit –m “1st file”
git push –set-upstream origin Develop
2) Change to a different branch and add some files and merge into main
when you are done.
git branch second
git checkout second
git branch
nano File1.txt
nano File2.txt
git add .
git status
git commit –m “created 2 files”
git checkout main
git merge second
3) Submit another pull request, with squashed commits.
git checkout Develop
git log
git rebase –i HEAD~1
git checkout
git checkout second
nano File3.txt
nano File4.txt
git add .
git commit –m “file 3-4”
git rebase –i HEAD~2
git push –set-upstream origin second



Task 3:
1) Сгенерируйте конфликт на main. Напишите решение
cd IdeaProjects/
mkdir Task3
cd Task3/
git clone https://github.com/whoismiras/Task3.git
nano 1.txt
git add 1.txt
git commit –m “1st file”
git push 
Создаем (имитируем) изменения файла на github.com
nano 1.txt
git add .
git commit –m “2nd file”
git pull
nano 1.txt
git add .
git commit “3”
git push
2) Потом сгенерируйте конфликт в бранче. Тоже напишите решение.
git branch Develop
nano 1.txt
git merge main
nano 1.txt
git add .
git commit –m “solved conflict”
git push



Task 4:
1)	Cоздать 2 файла, разделить их на 2 push
nano 2.txt
nano 3.txt
git add –p 2.txt
git commit –m “first push”
git push
git add –p 3.txt
git commit –m “second push”
git push



Task 5:
1)	Add 5 blocks of information into text, commit and push only 3 of them, without deleting any content.
nano 5.txt
git add –p 5.txt
git commit –m “blocks”
git push



